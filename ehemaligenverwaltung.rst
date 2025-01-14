

.. attention:: 🚧 Die hier bereitgestellten Informationen befinden sich noch in der Überarbeitung und sind möglicherweise unvollständig oder ungenau. Es können sich Änderungen ergeben, die den Inhalt dieser Dokumentation betreffen. Bitte verwende die hier enthaltenen Angaben mit Vorsicht oder wende dich direkt an das Netzwerk Ehemalige Jungwacht Blauring (NEJB).

===============
Ehemalige / NEJB
===============

Mit dem Release 2.3.15 (14.01.2025) hat das `Netzwerk Ehemalige Jungwacht Blauring (NEJB) <https://www.jubla.ch/ueber-die-jubla/ehemalige/netzwerk>`_ eine eigene Struktur in der Jubla Datenbank. Dieser «Top-Knoten» dient dem Netzwerk, den Ehemaligenvereinigungen und ihren Mitgliedern zur Mitgliederverwaltung. Aktive Ehemaligenvereinigungen können als Kollektivmitglieder des Netzwerks ihre Mitglieder, Netzwerkpartner und Dienstleister verwalten. Die jubla.db folgt damit dem Jubla-Verständnis von Lebensfreunden fürs Leben. 

.. figure:: /media/ehemalige/ehemalige_top-knoten.png
    :name: Ansicht der Top-Knoten Jubla Schweiz und Netzwerk Ehemalige Jungwacht Blauring (NEJB)

«Top-Knoten NEJB» des Netzwerk Ehemalige Jungwacht Blauring



Top-Knoten Ehemalige 
===============

Der «Top-Knoten Ehemalige» ist ein Technisches Konstrukt (Feature), verwaltet durch das Netzwerk Ehemalige Jungwacht Blauring. Mit Strukturen wie Ebenen (Kantone/Regionen) oder Ehemaligenvereinigungen können unter Koordination durch das Netzwerk die Ehemaligen-Vereine in der jubla.db aktiv sein und sich vernetzten. Das Netzwerk Ehemalige Jungwacht Blauring ist der nationale Verein, der das Ehemaligenwesen koordiniert. Als Ehemalige*r kannst du Mitglied werden und bekommst mit deinem jubla.db Profil eine Rolle in diesen Vereinen. Kantonale und regionale Ehemaligen-Vereinigungen können Kollektivmitglieder werden. Mehr: https://www.jubla.ch/ehemalige   

Hier werden technischen Funktionen erläutert im Hinblick auf Regeln, Automatismen und Abläufe, die den Austritt sowie den Übertritt ins Ehemaligenwesen innerhalb des eigenen Vereins oder in andere Vereine unterstützen.
Beachte, dass die hier beschriebenen Themen ergänzend zu den organisatorischen Abläufen und Regelungen gelten, die sich aus der Vereins- und Vorstandsarbeit ergeben. Diese findes du im `jubla.netz Vereinsmanagement <https://jubla.atlassian.net/wiki/x/DYArRg>`_.



Rolle «Austritt»
===============

Die Rolle «Ehemalig» wurde in «Austritt» umbenannt. Diese aktive Rolle wird automatisch vergeben, wenn die letzte Rolle entfernt wird. Üblicherweise signalisiert sie den Austritt aus einer Schar oder einer Ebene/Gruppe. Die Umbenennung in Austritt soll verdeutlichen, dass sie für die Zeit vorgesehen ist in der ein Mitglied (nicht nur auf lokaler Ebene) den Austritt angekündigt hat bis zu deren Umsetzung und Mutation. Die Folge davon: Wird der Austritt korrekt vollzogen, wird die Rolle «Austritt» vergeben. Austritte werden regelmässig (an der GV) verabschiedet und danach die Rolle «Austritt» vom Profil entfernt. Profile ohne Rollen werden danach dadurch zu ausgetretenen Leitungspersonen oder in die Gruppe «ohne Rollen» auf dieser Ebene verschoben. Das Profil hat danach die korrekte «Inaktive Rolle» in seinem Verlauf. Dies führt dazu, dass die Mitgliedschaft in einem Verein mit dem Austritt vollzogen werden kann. Mit dem Austritt ist das Profil danach korrekt kein Mitglied mehr und der Übertritt ins Ehemaligenwesen wird möglich.


Austritt Automatismus
===============


Eine Rolle bestimmt und beschreibt die Zugehörigkeit zu einer Gruppe (Verein). Wird von eine Profil eine Rolle entfernt, prüft das System, ob dieses noch weitere Rollen innerhalb der Gruppe hat. Falls zum Profil keine weiteren solchen Rollen gefunden werden, führt das System den Austritts-Automatismus aus.

- In Gruppen auf den Ebenen Kanton/Region/Bund vergibt dann das System dem Profil die Rolle "Austritt({Bisherige-Rolle})" in der bisherigen Gruppe z.B. " Austritt(Leiter/in)”.
- In Gruppen vom Typ Schar vergibt das System dem Profil ebenfalls die Rolle "Austritt({Bisherige-Rolle})". Zusätzlich dazu wird dem Profil die Rolle Mitglied innerhalb der Schar in der Untergruppe "Ausgetretene Leitungspersonen" vergeben. 

Regeln für den Automatismus:

- Das Profil hat keine Inaktive-, Ehemaligen- oder Austritt-Rolle in der Gruppe/Ebene/Verein
- Die gelöschte Rolle war mindestens 7 Tage vergeben (sonst wird die Rolle bei der Löschung als "Versehen" angesehen und komplett gelöscht, ohne eine Ehemaligenrolle zu erstellen (landet in «ohne Rollen)
- Kinder unter 15 Jahren sind vom Automatismus ausgeschlossen: Bei gelöschten Rollen aus Kindergruppen muss im Profil über das Geburtsdatum ein Alter von mindestens 15 Jahren vorliegen. 



Bedingungen für E-Mail "Ehemalige: Benachrichtigung Schar" 
===============

Ein Profil wird mit über den Automatismus benachrichtigt. Dafür müssen folgende Bedingungen efüllt sein:

- Das Profil hat eine gültige Haupt-E-Mail   
- Die letzte aktive Rolle der Person in dieser Schar wird entfernt/gelöscht oder wird per Bis-Datum ungültig.   
- Das Profil hat noch keine Ehemaligenrolle(n) (inaktive Rollen) in dieser Ebene/Schar
- Die gelöschte Rolle war mindestens 7 Tage alt (sonst wird die Rolle bei der Löschung als "Versehen" angesehen und komplett gelöscht ohne eine Ehemaligenrolle zu erstellen oder Mails zu versenden) 
- Kinder unter 15 Jahren erhalten keine E-Mail. Bei Rollen aus Kindergruppen muss im Profil über das Geburtsdatum ein Alter von mindestens 15 Jahren vorliegen. 
- 1 Tag ist seit dem Löschen der Aktivrolle vergangen, und die Ehemaligenrolle existiert immer noch. 




Gruppe «Ausgetretene Leitungspersonen» auf ebene Schar
===============

Die automatisch erstellte Gruppe «Ausgetretene Leitungspersonen» auf Scharebene ist ein Auffangbecken für Menschen welche früher eine Rolle (wie zum Beispiel «Leiter/in») in der Schar hatten. Die Schar bleibt weiterhin mitverantwortlich für diese Profile als Netzwerkpartner. 

