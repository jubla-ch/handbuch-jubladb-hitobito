.. _changelog-news:

News zu Releases der Jubla Datenbank
============================



.. hint:: Im Changelog der Applikation (https://db.jubla.ch/changelog) ist die jeweilige Version und die vorgenommenen Aktualisierungen dokumentiert. Bei einem Release/Update wird die Datenbank jeweils für kurze Zeit gesperrt, gewartet und mit neuen Funktionen ausgestattet. Hier werden die jeweils wichtigsten Veränderungen für Jungwacht Blauring erwähnt.
Geplante Release-Daten für die jubla.db: 
1/24 - Di, 09. Januar - Quartalsrelease Hitobito/jubla.db 
2/24 - Di, 2. April - Quartalsrelease Hitobito/jubla.db 
3/24 - Di, 2. Juli - Quartalsrelease Hitobito/jubla.db 
4/24 - Di, 01. Oktober - Quartalsrelease Hitobito/jubla.db 




Release Version 2.0 (1.30) / 09.01.2024
----------------------------

Release-Kommunikation von Hitobito: https://mailchi.mp/4e0e63733071/herbstliche-grsse-von-hitobito-6685199 

- Elternzugang
Seit dem Release ist die technische Grundlage bereit um in der Datenbank Eltern oder Erziehungsberechtigte so zu erfassen, dass sie Zugriff auf ihre Kinder haben. Dank dieser Funktion ist eine Einsicht in die Daten der Kinder und deren Anmeldung zu Anlässen, Kursen und Lagern möglich. Eltern benötigen ab jetzt nur ein Profil (und eine E-Mail-Adresse), um mehrere Kinder verwalten zu können.

- Nextcloud
Die jubla.db besitzt nund die technische Grundfunktion, damit sich Profile aus der Datenbank direkt in eine Nextcloud-Instanz im Besitz einer Ebene (Schar/Verein) anmelden kann. 

- Frontend-Toolkit Bootstrap 5
Das Frontend-Toolkit Bootstrap wurde von der Version 2 auf 5 aktualisiert. Die Darstellung (Frontend) der Applikation profitiert davon.

- Ruby 3.0
Mit diesem Release erfolgt ein Upgrade auf Ruby 3.0. Es hat keinen Einfluss auf das Verhalten oder Funktionen der jubla.db, ist eber für die Sicherheit und Zukunftskompatibilität wichtig.

- Gruppen/Schar-Tab "Einstellungen" 
Der Tab "Einstellungen" auf Ebene Schar/Kanton/etc. wurde entfernt und die Optionen (Briefe/SMS-Provider) sind neu in der Bearbeitungsansicht der Gruppe unter dem Tab "Abos". 

- Seite für Selbstregistrierung
Neu gibt es für die Schar (Gruppen) mit aktivierter Selbstregistrierung eine Seite, über welche sich auch eingeloggte Personen in der Gruppe einschreiben können. Menschen ohne Profil wird weiterhin die bisherige Seite für eine externe Registrierung angezeigt.

- Zugriffs Ansicht im Tab Sicherheit
Der Sicherheits-Tab eines Profil kann neu die Gruppen und Rollen auflisten, welche Zugriff auf einem haben.

- Abos einfacher zuweisen
Auf der Personen-Listenansicht können neu via Multiselekt Personen als Abonnenten einem Abo hinzugefügt werden. Abos können so einfacher und schneller erstellt oder verwaltet werden.

- Datenschutzerklärung pro Ebene 
Neu kann auf einer Ebene eine Datenschutzerklärung (DSE) hinterlegt werden. Diese muss, falls vorhanden, bei der Selbstregistrierung, dem Anmelden bei einem Anlass/Kurs oder dem Hinzufügen einer Person auf einer Gruppe akzeptiert werden um fortzufahren. Informationen zum Datenschutz im jubla.netz: https://jubla.atlassian.net/l/cp/FgNbRw1v 

- Export gemäss BSV-Regeln
Der BSV-Export berücksichtigt jetzt gemäss den neuen BSV-Regeln alle Personen unter 30 Jahren (statt wie zuvor nur zwischen 17 und 30 Jahren).



Release Version 1.28 / 15.11.2022
----------------------------

- Kursfilter
In der Kursübersicht in der Datenbank können die Kurse neu gefiltert werden. Standardmässig werden die Kurse des eigenen Kantons und der nationalen Ebene angezeigt. Die ausserkantonalen Kurse sind via DropDown auffindbar, die Suche nach alternativen Kursangeboten wird einfacher. Wer den Kurs durchführt, ist neu in der Übersicht direkt sichtbar. Weiterhin ist die Sichtbarkeit von Kursen und Veranstaltungen über die Option "Anlass ist für die ganze Datenbank sichtbar" einstellbar.

- J+S Reaktivierung von Qualifikationen
Das Bundesamt für Sport BASPO hat Änderungen an der Reaktivierung von Qualifikationen vorgenommen, der Status “weggefallen archiviert” wurde aufgehoben (Siehe hier). Die Datenbank kommt nun mit diesen neuen Bedingungen zurecht. Die Vorbedingungen einer Kursart können deshalb neu als "Muss gültig sein" oder "Muss gültig oder weggefallen sein" deklariert werden. Wenn die Vorbedingung gültig sein muss, verhält es sich wie bisher, bei gültig oder weggefallen muss der*die Teilnehmer*in die Qualifikation der Vorbedingung besitzen oder jemals besessen haben. Dies gilt unabhängig von der Gültigkeit oder Reaktivierbarkeit der besagten Qualifikation.

- Rollen in Kursen und deren Qualifikationsverlängerung (NDS)
Im Dezember 2022 wird die neue Nationale Datenbank für Sport (NDS) ihren Betrieb aufnehmen. Für die korrekte Übertragung der Qualifikationsverlängerungen sind nun Anpassungen an den Rollen notwendig. Die Rolle «Kurshelfer*in» ist neu für Personen vorgesehen, welche mindestens 6h Kadertätigkeit ausüben. Die Rolle «Referent*in» für weniger als 6h Kadertätigkeit. Im Bereich «Qualifikationen» sind deshalb neu nebst Hauptleitung und Leitung auch «Helfer*innen» aufgeführt. Ihnen können nun auch die Qualifikationen verlängert werden. 

- Berechtigungen der Rolle Coach angepasst
Die Rolle «Coach» kann neu neben der Hauptleitung (Lagerleitung) und Leitung ebenfalls die Lager-Teilnehmenden-Liste exportieren (CSV Datei SPORTdb/NDS) und gemäss Vorgaben verwenden. 

- Wer ist wo im Lager
Die kantonalen/regionalen Arbeitsstellen und die nationale Geschäftsstelle haben über ein neues Modul “Lager” eine Übersicht über die Lager in ihrer jeweiligen Ebene, sofern das Lager als “sichtbar” angelegt wurde. Die Möglichkeit zur Koordination oder Unterstützung wird so unterstützt. 

- Personentab Sicherheit
Berechtigte Personen, wie zum Beispiel die Scharleitung, können den Personentab für Sicherheit und Datenschutz verwenden.



Release Version 1.27 / 12.07.2022
----------------------------

- Gruppen-Kalender 
In den Einstellungen jeder Gruppe lassen sich neu Kalender-Feeds einrichten. So können Anlässe, Kurse, Jahrespläne etc. im eigenen Kalender (z.B. in deinem Smartphone-Kalender oder im Outlook) eingebunden werden. Das Smartphone oder die Applikation muss dazu die Funktion «Importieren oder Abonnieren eines Kalenders per URL» haben. 
Rollen mit Start- und Enddatum 
Rollen können beim Erstellen und Editieren neu ein Start- und Enddatum erhalten. In der Zukunft liegende Daten passen dann die Rolle automatisch an. Beim Planen darauf achten, dass eine Person nicht ungewollt alle Rollen verliert. Siehe auch jubla.db-Erweiterung für Ehemalige. 

- Anlässe 
Kontaktpersonen können sich über neue Anmeldungen per E-Mail benachrichtigen lassen. Die Option kann in den Einstellungen für einen Termin aktiviert werden. Hier lassen sich auch neu Tags für Anlässe, Kurse oder Lager setzten. 

- Sicherheit 
Der persönliche Zugang zur Datenbank kann optional mit einem «Time-based One-Time Password» (TOTP/2FA) zusätzlich geschützt werden. Apps wie FreeOTP von Red Hat (OpenSource), google Authenticator oder Microsoft Authenticator können den zusätzlichen Zahlencode für das Login generieren. Sichere deine Zugangsdaten so, dass du beim Verlust deines Smartphones den Zugang zur Datenbank nicht verlierst.  
Die Haupt-E-Mail-Adresse (wird als Login verwendet) muss zukünftig bei Änderungen bestätigt werden.  


Release Version 1.26 / 07.12.2021
----------------------------

- Verlängerung der Qualifikationen parallel zu J+S
Die ausserordentliche Verlängerung der Einsatzberechtigung von J+S-Leiter*innen wird in der Datenbank bei den betroffenen Personen auf «gültig bis 31.12.2022» mutiert.

- Passwort-Richtlinie gemäss aktuellen Empfehlungen 
Bestehende Passwörter bleiben unverändert gültig. Neue Passwörter müssen mindestens 12 Zeichen lang sein. Weiterhin werden keine Vorgaben für Zahlen, Sonderzeichen, Gross- und Kleinschreibung gemacht.

- Kursfilter für Kursansicht 
Neu können Kurse zusätzlich nach verschiedenen Kriterien wie Datum, Gruppen, Kursart, Kurskategorie oder freien Plätzen gesucht werden.

- Sichtbarkeit von Anlässen / Kursen / Lagern 
Anlässe, Kurse und Lager sind neu ans Berechtigungssystem der Benutzer*innen angeglichen und nicht mehr für alle sichtbar. Bei Bedarf kann ein Anlass weiterhin für die ganze Datenbank sichtbar gemacht werden.

- Einladungen zu Anlässen & Lagern in der Datenbank 
Neu sind Einladungen zu Anlässen und Lagern möglich. Die eingeladene Person sieht dann auf der Info-Seite des entsprechenden Events eine Auswahl, um sich an- oder abzumelden. 

- Teilnehmersichtbarkeit: Gegenseitige Sichtbarkeit von Teilnehmer*innen von Anlässen 
Neu kann für jeden Anlass, jeden Kurs und jedes Lager separat konfiguriert werden, ob sich die angemeldeten Teilnehmer*innen gegenseitig sehen. (Standardmässig ist die Sichtbarkeit deaktiviert)
Du hast Fragen oder kommst du nicht weiter? Dann melde dich bei deiner kantonalen/regionalen Arbeitsstelle. 
