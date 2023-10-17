# frozen_string_literal: true

namespace :sources do
  task extract: ['sphinx/bin/sphinx-build'] do
    sh 'sphinx/bin/sphinx-build -b gettext . _build/gettext'
  end

  desc 'Update gettext and config from the source and push to transifex'
  task update: %i[sources:extract tx:config tx:push]
end

namespace :translations do
  desc 'Pull translations from transifex and commit'
  task update: %i[tx:pull] do
    sh 'git add locales/'
    sh 'git commit -m "Update translations from transifex"'

    puts 'You can now push the docs, so the website can be rebuilt.'
  end
end

namespace :tx do
  task push: ['bin/tx'] do
    sh 'bin/tx push --source'
  end

  task pull: ['bin/tx'] do
    sh 'bin/tx pull --translations --all --force'
  end

  task :config do
    Rake::Task['.tx/config'].execute
  end

  task status: ['bin/tx'] do
    sh 'bin/tx --version'
    sh 'bin/tx status'
  end
end

namespace :build do
  task all: %i[en it fr]

  task :en do
    Rake::Task['build:docs'].execute(locale: 'en')
  end

  task :it do
    Rake::Task['build:docs'].execute(locale: 'it')
  end

  task :fr do
    Rake::Task['build:docs'].execute(locale: 'fr')
  end

  task :docs, [:locale] => ['sphinx/bin/sphinx-build'] do |_t, args|
    locale = args[:locale]

    sh "sphinx/bin/sphinx-build -b html -D language=#{locale} . _build/html/#{locale}"
  end
end

directory 'bin/'

file 'bin/tx': ['bin/'] do
  transifex_version = 'v1.6.4'

  sh "curl -L https://github.com/transifex/cli/releases/download/#{transifex_version}/tx-linux-amd64.tar.gz | " \
    'tar xz -C bin/'
end

directory '.tx/'

file '.tx/config': ['.tx/'] do |task|
  organization = 'hitobito'
  project = 'user_documentation'
  source_lang = 'de'

  header = <<~INI
    [main]
    host = https://www.transifex.com

  INI

  template = <<~INI
    [o:#{organization}:p:#{project}:r:<resource>]
    file_filter = locales/<lang>/LC_MESSAGES/<resource>.po
    source_file = _build/gettext/<resource>.pot
    source_lang = #{source_lang}
    type        = PO

  INI

  File.open(task.name, 'w') do |config|
    config << header

    FileList['_build/gettext/*.pot'].each do |source|
      config << template.gsub('<resource>', File.basename(source, '.pot'))
    end
  end
end

directory 'sphinx/' do
  sh 'virtualenv sphinx'
end

file 'sphinx/bin/sphinx-build': ['sphinx/'] do
  sh 'sphinx/bin/pip install sphinx_rtd_theme' # ensure correct dependency resolution
  sh 'sphinx/bin/pip install sphinx sphinx-intl[transifex]'
end
