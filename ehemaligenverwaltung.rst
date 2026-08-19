===============================
Ehemaligenverwaltung
===============================

Diese Seite erklärt dir als Scharleitung/Adressverwaltung, wie die Datenbank mit Ehemaligen umgeht und wie du diese einsehen kannst.

Rolle «Austritt» – Was ist das?
===============================

Wenn jemand aus einer Schar/Gruppe austritt, bekommt diese Person automatisch die Rolle **«Austritt»** zugewiesen. 

Das bedeutet:
- Die Person ist **nicht mehr aktiv** in der Schar
- Die Person hat **keine aktiven Rollen** mehr (wie «Leiter/in», «Kassierer/in», etc.)
- Du kannst die Person trotzdem **einsehen** und **kontaktieren** (wenn sie die Kontaktfreigabe erlaubt hat)

**Wichtig:** Die Rolle «Austritt» wird automatisch vergeben, sobald eine Person ihre letzte aktive Rolle in einer Gruppe verliert. Du musst nichts tun – das läuft automatisch ab.

Wo sehe ich Ehemalige?
======================

Du kannst Ehemalige im Reiter **«Austritte»** einsehen.

So funktioniert’s:

1. Öffne deine Schar in der jubla.db
2. Gehe zum Abschnitt **«Personen»**
3. Dort findest du mehrere Reiter oben:
   - «Mitglieder» (alle Personen mit aktiven Rollen)
   - **«Austritte»** (alle Personen ohne aktive Rollen)
   - Weitere Reiter je nach Rolle
4. Klicke auf **«Austritte»**
5. Dort siehst du alle Personen, die die Rolle «Austritt» haben

**Tipp:** Du kannst diese Liste durchsuchen, filtern und exportieren wie jede andere Liste in der DB.

Worauf sollte ich achten?
=========================

- **Kontaktfreigabe:** Nicht alle Ehemaligen möchten kontaktiert werden. Prüfe ihre Kontaktfreigabe.
- **Datenschutz:** Respektiere die Datenschutz-Einstellungen der Personen
- **Netzwerk:** Ehemalige, die sich im Netzwerk organisieren möchten, machen das über Ehemaligenvereine (siehe unten)

Wie funktioniert der Automatismus «Austritt»?
=========================
Eine Rolle bestimmt und beschreibt die Zugehörigkeit zu einer Gruppe (Verein). Wird von einer Person eine Rolle entfernt, prüft die Datenbank, ob diese noch weitere Rollen innerhalb der Gruppe hat. Falls zur Person keine weiteren solchen Rollen gefunden werden, führt die Datenbank den Austritts-Automatismus aus.

In Gruppen auf den Ebenen Kanton/Region/Bund vergibt dann das System dem Profil die Rolle «Austritt ({Bisherige-Rolle})» in der bisherigen Gruppe, z. B. *«Austritt (Leiter/in)»*.

In Gruppen vom Typ Schar vergibt das System der Person ebenfalls die Rolle «Austritt ({Bisherige-Rolle})». Zusätzlich dazu wird der Person die Rolle «Mitglied» innerhalb der Schar in der Untergruppe «Austritte» vergeben.

Regeln für den Automatismus:

Die Person hat keine Inaktive-, Ehemaligen- oder Austritt-Rolle in der Gruppe/Ebene/Verein.

Die gelöschte Rolle war mindestens 7 Tage vergeben (sonst wird die Rolle bei der Löschung als «Versehen» angesehen und komplett gelöscht, ohne eine Ehemaligenrolle zu erstellen (landet in «ohne Rollen»)).

Kinder unter 15 Jahren sind vom Automatismus ausgeschlossen: Bei gelöschten Rollen aus Kindergruppen muss im Profil über das Geburtsdatum ein Alter von mindestens 15 Jahren vorliegen.

E-Mail «Ehemalige: Benachrichtigung Schar» - *Danke für dein Jubla-Sein*
----------------------------------------

Wird der Automatismus mit einer Person auf Ebene Schar durchgeführt, erhält diese eine E-Mail. Darin wird sie gebeten, ihre Kommunikationspräferenzen zu prüfen (siehe :doc:`Kontaktfreigabe <ehemalige/kontaktfreigabe>`). 
Damit das Mail ausgelöst wird, müssen folgende Bedingungen erfüllt sein:

- Das Profil hat eine gültige Haupt-E-Mail

- Die letzte aktive Rolle der Person in dieser Schar (in der Hauptgruppe oder Kindergruppe) wird entfernt/gelöscht oder wird per Bis-Datum ungültig.

- Das Profil hat noch keine inaktiven Rollen (Ehemaligenrollen) in dieser Ebene/Schar.

- Die gelöschte Rolle war mindestens 7 Tage alt.

- Im Gruppentyp Kindergruppe wird das Alter geprüft. Bei Rollen aus Kindergruppen muss im Profil über das Geburtsdatum ein Alter von mindestens 15 Jahren vorliegen.

- 1 Tag ist vergangen und das Profil hat in der Zwischenzeit keine neue aktive Rolle in dieser Schar erhalten.

Ehemaligenvereine im Netzwerk
==============================

Viele Scharen/Regionen/Kantone haben **Ehemaligenvereine**, die sich in der jubla.db organisieren.

Wenn du einen Ehemaligenverein leitest, findest du hier mehr Informationen: :ref:`Verwaltung von Ehemaligenvereinen <adressverwaltung-ehemalige>`

Dort erfährst du:

- Wie du eine Gruppe anlegst
- Wie du Mitglieder hinzufügst
- Wie du den Verein verwaltest
- Wie du Selbstregistrierungslinks erstellst


Häufige Fragen
===============

**F: Kann ich Ehemalige selbst in eine Ehemaligenvereins-Gruppe verschieben?**

A: Nein. Personen müssen sich selbst anmelden oder von der Vereinsleitung hinzugefügt werden. Du kannst diese Person aber auf den Ehemaligenvereins hinweisen.

**F: Was ist der Unterschied zwischen «Austritt» und «Ehemalige»?**

A: In der jubla.db sind diese Begriffe synonym – beide bedeuten, dass die Person nicht mehr aktiv ist. Die Rolle heisst «Austritt», die Person wird aber als «Ehemalige*r» bezeichnet.

**F: Kann ich eine Person manuell in den Reiter «Austritte» hinzufügen?**

A: Nein, das funktioniert automatisch. Die Person muss zuerst ihre letzte aktive Rolle verlieren, dann wird die Rolle «Austritt» automatisch vergeben.

**F: Kann ich Ehemalige wieder in die aktive Schar aufnehmen?**

A: Ja! Du kannst der Person eine neue aktive Rolle zuweisen (z. B. «Leiter/in»). Dann wird die Rolle «Austritt» gelöscht und die Person ist wieder aktiv.

Kontakt & weitere Hilfe
=======================

Fragen zu Ehemaligenverein-Verwaltung? 

→ Kontakt: db@ehemaligejubla.ch

Weitere Dokumentation zum Thema Ehemalige: :doc:`Ehemalige – Dokumentation <ehemalige/index>`