..  _lagerverwaltung-link-target:

========================
Lagerverwaltung
========================
Dieser Anleitungsbereich dient der Lagerleitung und Personen, welche für die Lagerverwaltung in deiner Schar zuständig sind. Der erste Teil handelt davon, wie du ein neues Lager erstellen und konfigurieren kannst. Der zweite Teil behandelt die Lageranmeldung. 

Lagerübersicht
==============

Über die Registerkarte ``Lager`` im Modul ``Gruppen`` gelangst du zur Übersicht aller erfassten Lager deiner Schar.

.. figure:: /media/lagerverwaltung/gruppe_lager_uebersicht.png
    :name: 
    
    Lagerverwaltung - Übersicht

Hier findest du verschiedene Schaltflächen zur Lagerverwaltung mit den folgenden Funktionen:

* **Lager erstellen**: Mit :guilabel:`Lager erstellen` öffnet sich ein neues Fenster, in dem ein neues Lager erstellt werden kann.  
* **Export**: Mit :guilabel:`Export` können die Lagerinformationen entweder im CSV-Dateiformat oder in einem Excel exportiert werden.
* **Kalender Export**: Mit :guilabel:`Kalender Export` wird das Lager automatisch in ein ICS-Dateiformat umgewandelt und im Browser heruntergeladen. Diese ICS-Datei kann schlussendlich in einen digitalen Kalender wieder importiert und eingefügt werden.
* **Historie & Filtern**: Die Filterfunktion oben links und die Historie oben rechts helfen dir dabei, ein bestimmtes Lager zu finden.

Lager erstellen
===============

Damit du ein neues Lager auf der Datenbank erstellen kannst, benötigst du die Rolle ``Lagerleitung`` oder ``Scharleitung``. Hast du eine dieser beiden Rollen, kannst du durch Anwählen von :guilabel:`Lager erstellen` ein neues Lager anlegen. Nach dem Klicken öffnet sich ein Fenster mit mehreren Registern, in denen du individuelle Konfigurationen vornehmen kannst. Generell gilt, dass die mit ***** markierten Felder zwingend ausgefüllt werden müssen. Die anderen sind optional.

.. figure:: /media/lagerverwaltung/gruppe_lager_erstellen.png
    :name: 
    
    Lagerverwaltung - Lager erstellen

Allgemein
~~~~~~~~~~

Im Register ``Allgemein`` können Informationen wie **Name**, **Lagerart**, **Motto**, **Kosten**, **Ort/Adresse** und **Coach** eingetragen werden.

.. figure:: /media/lagerverwaltung/lager-erstellen_uebersicht.png
    :name: 
    
    Lagerverwaltung - Allgemein

Zudem kann Folgendes definiert werden:

* **Nummer**: Hier kann die J+S‑Nummer eingetragen werden.
* **Beschreibung**: Hier können Einverständnisabklärungen eingefügt werden (Datenschutz, Bildrechte etc.). Diese werden auf der Rückseite der :ref:`Anmeldebestätigung <anmeldebestätigung-link-target>` aufgelistet, welche nach dem Absenden der Anmeldung an die angegebene Mailadresse gesendet und durch eine Unterschrift bestätigt wird, sofern unter :ref:`Anmeldung <anmeldung-link-target>` der Haken bei "Unterschrift erforderlich" gesetzt ist. Vorschläge findest du auf `jubla.netz/Lageranmeldung <https://jubla.atlassian.net/wiki/spaces/WISSEN/pages/1478819847/Lageranmeldung>`_ unter "Kleingedrucktes".
* **Kontaktperson**: Hier kann eine Kontaktperson für das Lager ausgewählt werden. Nach dem Auswählen öffnen sich Anzeigeoptionen, die festlegen, welche Informationen der Kontaktperson auf der jula.db angezeigt werden.
* **Sichtbarkeit**: Mit dem Aktivieren von "Anlass ist für die ganze Datenbank sichtbar" ermöglichst du anderen Scharen, sich für euer Lager anzumelden.

Daten
~~~~~~

Unter ``Daten`` wird der Zeitraum des Lagers definiert.

.. figure:: /media/lagerverwaltung/lager-erstellen_daten.png
    :name: 
    
    Lagerverwaltung - Daten

* **Von**/**Bis**: Start- und Enddatum des Lagers.
* **Bezeichnung**: Beispielsweise: Sommerlager.
* **Ort**: Adresse vom Lagerplatz.
* **Eintrag hinzufügen**: Falls dein Lager in zwei Abschnitte aufgeteilt ist, kann mit ``Eintrag hinzufügen`` eine weitere Zeitspanne definiert werden.

..  _anmeldung-link-target:

Anmeldung
~~~~~~~~~~

Im Register ``Anmeldung`` definierst du alles Organisatorische für deine Lageranmeldung.

.. figure:: /media/lagerverwaltung/lager-erstellen_anmeldung.png
    :name: 
    
    Lagerverwaltung - Anmeldung

* **Anmeldebeginn/Anmeldeschluss**: Hier kannst du den Anmeldezeitraum bestimmen.
* **Aufnahmebedingungen**: Falls dein Lager Anforderungen an die Teilnehmenden stellt, wie zum Beispiel ein Mindestalter, kannst du das hier definieren.
* **Teilnehmendenzahl**: Mit den Feldern ``Maximale-/Minimale Teilnehmendenzahl`` kann die Personenanzahl gesteuert werden. Wenn die maximale Anzahl bereits vor dem Anmeldeschluss erreicht wird, so wird das Anmeldefenster automatisch vorzeitig geschlossen.
* **Externe Anmeldungen**: Wenn aktiviert, können sich auch Personen, welche noch kein Profil auf der jubla Datenbank haben, für dieses Lager anmelden. Falls du vorhast, dass die Erziehungsberechtigten ihre Kinder selbst über den :ref:`Elternzugang <elternzugang-link-target>` anmelden, empfiehlt es sich, dieses Feld zu deaktivieren. So wird sichergestellt, dass die Eltern sich mit dem richtigen Profil anmelden.
* **Teilnehmersichtbarkeit**: Hier kann festgelegt werden, ob die Teilnehmenden sehen können, wer sich für das Lager angemeldet hat.
* **(Zweit)Unterschrift erforderlich**: Aktivierung von ``Unterschrift erforderlich`` fordert die Teilnehmenden nach der Anmeldung auf, die Anmeldebestätigung, welche per Mail zugestellt wird, zu unterschreiben und an die Kontaktperson zu senden. Falls eine Zweitunterschrift benötigt wird, zum Beispiel von einer erziehungsberechtigten Person, kann ``Zweitunterschrift erforderlich`` zusätzlich aktiviert werden.
* **Abmeldung**: Die Teilnehmenden können sich selbst abmelden.
* **Anmeldebemerkungen**: Hier können Hinweise zur Anmeldebestätigung angegeben werden, zum Beispiel bis wann und auf welchem Weg die unterschriebene Anmeldebestätigung retourniert werden soll.

..  _anmeldeangaben-link-target:

Anmeldeangaben
~~~~~~~~~~~~~~~~

Unter ``Anmeldeangaben`` kannst du hilfreiche Informationen über die Teilnehmenden einholen, wie zum Beispiel das Schwimmniveau, die Essgewohnheiten, die T-Shirt-Grösse etc. Durch Klicken auf ``Eintrag hinzufügen`` kannst du neue Fragen erstellen, welche die Teilnehmenden bei der Anmeldung oder die Lagerleitung beim Hinzufügen neuer Personen beantworten müssen. Auf `jubla.netz/Lageranmeldung <https://jubla.atlassian.net/wiki/spaces/WISSEN/pages/1478819847/Lageranmeldung>`_ findest du unter "Allgemeine Angaben" Empfehlungen dazu, welche Informationen du dir einholen solltest.

.. figure:: /media/lagerverwaltung/lager-erstellen_anmeldeangaben.png
    :name: 
    
    Lagerverwaltung - Anmeldeangaben

* **Frage**: Hier kannst du die Frage definieren.
* **Antwortmöglichkeiten**: Durch ``Antwortmöglichkeit hinzufügen``, können Antworten vorgegeben werden. Für Freitextantworten kannst du die Antwortmöglichkeiten weglassen. Wenn mehrere Antworten möglich sein sollen, ``Mehrfachauswahl`` aktivieren.
* **Obligatorisch**: Durch das Anwählen muss diese Frage zwingend beantwortet werden.
* **Sichtbar für**: Hier kannst du festlegen, welche Personen die Berechtigung erhalten, die Antworten der Teilnehmenden zu sehen. So kannst du etwa Mitgliedern der Küche die Berechtigung für die Frage der Essgewohnheiten geben. Wenn du die Antworten für die Teilnehmer*innen zugänglich machen willst, muss zusätzlich im vorherigen Abschnitt ``Anmeldung`` der Haken unter ``Teilnehmersichtbarkeit`` gesetzt sein. Ansonsten gelangen sie nicht auf die Teilnehmeransicht, auf der die Informationen aufgeführt sind.

    **Beispiel - Sichtbarkeit**:
    
    In der folgenden Abbildung siehst du, wie die Teilnehmerübersicht unter dem Register ``Teilnehmende`` aus der Sicht eines Küchenmitglieds (Sebastian Muster) aussehen kann. Um die Antworten der Teilnehmenden zu sehen, muss unter ``Spalten`` die entsprechende Frage ausgewählt werden. In diesem Beispiel kann die Person nur die Essgewohnheiten einsehen, jedoch nicht das Schwimmniveau (ausser ihr eigenes).
    
    .. figure:: /media/lagerverwaltung/lager-erstellen_anmeldeangaben_tnübersicht_küche.png
        :name: 
            
        Lagerverwaltung - Teilnehmerübersicht als ``Küche``

    Anschliessend können die Informationen über ``Export`` als Excel heruntergeladen werden, um etwa die Menüplanung digital vorzunehmen.

.. important:: Wenn du vorhast, die :ref:`Lageranmeldung über den Elternzugang <lageranmeldung_elternzugang-link-target>` durchzuführen, darfst du den Haken bei den Fragen nicht auf obligatorisch setzen. Ansonsten kann die Anmeldung nicht abgeschlossen werden, da ihnen die Anmeldeangaben nicht angezeigt werden und sie diese nicht beantworten können. Sie werden aber auf der Anmeldebestätigung aufgeführt und können analog beantwortet werden, einfach ohne vordefinierte Antwortmöglichkeiten.

.. important:: *28.09.2026* ~Problem: Anmeldeangaben werden Eltern beim Ausfüllen der Lageranmeldung für ihre Kinder über den Elternzugang nicht angezeigt. Ist eine Frage obligatorisch, kann die Anmeldung nicht abgeschlossen werden. -> Anmeldeangaben sollen auch für die Eltern beim Anmelden ihrer Kinder sichtbar sein.

..  _administrationsangaben-link-target:

Administrationsangaben
~~~~~~~~~~~~~~~~~~~~~~

Im Abschnitt ``Administrationsangaben`` kannst du administrative Fragen erstellen. Im Gegensatz zu den Fragen unter ``Anmeldeangaben`` werden diese den Teilnehmer*innen bei der Lageranmeldung **nicht** gestellt, sondern lediglich der Lagerleitung, wenn sie neue Personen dem Lager hinzufügt oder bestehende Anmeldungen bearbeitet. So können etwa die Teilnehmer*innen durch die Lagerleitung in Lager- und/oder Ämtligruppen eingeteilt werden.

Wenn die Lageranmeldung durch die Teilnehmer*innen selbst ausgefüllt wird, werden nur die Fragen unter ``Anmeldeangaben`` angezeigt. Die Lagerleitung kann in diesem Fall die Administrationsfragen selbst nachträglich in der Anmeldung ergänzen.

.. figure:: /media/lagerverwaltung/lager-erstellen_administrationsangaben.png
    :name: 
    
    Lagerverwaltung - Administrationsangaben

* **Frage**: Hier kannst du die Frage definieren.
* **Antwortmöglichkeiten**: Durch ``Antwortmöglichkeit hinzufügen``, können Antworten vorgegeben werden. Für Freitextantworten kannst du die Antwortmöglichkeiten weglassen. Wenn mehrere Antworten möglich sein sollen, ``Mehrfachauswahl`` aktivieren.
* **Obligatorisch**: Durch das Anwählen muss diese Frage zwingend beantwortet werden.
* **Sichtbar für**: Hier kannst du festlegen, welche Personen die Berechtigung erhalten, die Administrationsantworten zu sehen. So kannst du etwa Mitgliedern der Küche die Berechtigung geben, die Gruppeneinteilung einzusehen, um diese für die Abwaschgruppeneinteilung zu verwenden.

.. important:: Wenn du vorhast, die :ref:`Lageranmeldung über den Elternzugang <lageranmeldung_elternzugang-link-target>` durchzuführen, oder wenn sich die :ref:`Teilnehmenden selbst für das Lager anmelden <teilnehmende_melden_sich_selbst_an-link-target>`, darfst du den Haken nicht auf obligatorisch setzen. Ansonsten kann die Anmeldung nicht abgeschlossen werden, da ihnen die Administrationsfragen nicht angezeigt werden und sie diese nicht beantworten können.

.. important:: *28.09.2026* ~Problem: Ist eine Administrationsfrage obligatorisch, kann die Anmeldung weder durch die direkte Lageranmeldung der TN noch durch eine Verwalter*in (Erziehungsberechtigte) abgeschlossen werden, da ihnen die Frage ja absichtlich nicht angezeigt wird. -> Anmeldung soll trotz obligatorische Administrationsangabe abschliessbar sein oder Administrationsfragen nicht als obligatorisch definierbar.
.. important:: *28.09.2026* ~Idee: -> Administrationsfragen können spezifisch für Leiter*innen oder Küchenmitglieder sichtbar gemacht werden, so könnten Leiterinformationen wie zum Beispiel "Kannst du Auto fahren?" oder "Hast du ein SLRG-Brevet?" abgefragt werden.
.. important:: *28.09.2026* ~Schreibfehler: Diese Frage muss beim Anmelden **beantworten** werden. -> Diese Frage muss beim Anmelden **beantwortet** werden.

..  _kontaktangaben-link-target:


Kontaktangaben
~~~~~~~~~~~~~~

Hier kannst du wählen, welche Kontaktangaben der Teilnehmenden bei der Anmeldung abgefragt werden sollen. Es gibt die Möglichkeit, zwischen ``Obligatorisch``, ``Optional`` und ``Nicht anzeigen`` zu wählen. Wenn du die Teilnehmenden als Lagerleiter*in selber hinzufügst, werden die Kontaktangaben nicht abgefragt. Willst du Kontaktangaben der Teilnehmenden hinzufügen oder verändern, musst du sie im jeweiligen Profil anpassen.

.. figure:: /media/lagerverwaltung/lager-erstellen_kontaktangaben.png
    :name: 
    
    Lagerverwaltung - Kontaktangaben

.. important:: Die folgenden Angaben sind obligatorisch für die NDS: **Name**, **Vorname**, **Geburtsdatum**, **Geschlecht** (nur weiblich oder männlich zulässig auf der NDS), **AHV-Nr.**, **Nationalität**, **Muttersprache**, **Strasse**, **Hausnummer**, **PLZ**, **Ort**, **Land**.

.. important:: *28.09.2026* ~Problem: Kontaktangaben werden aktuell nicht abgefragt, wenn die Lagerleitung TN selbst hinzufügt. Lagerrelevante Kontaktangaben müssen so vorgängig oder nachträglich im Profil ergänzt werden. -> Kontaktangaben werden auch beim Hinzufügen von TN durch Lagerleitung abgefragt.

Anleitungsvideo
~~~~~~~~~~~~~~~~~~

Falls du bei der Lagererstellung lieber einem Video folgst, kannst du dir dieses :fa:`video` `Anleitungsvideo <https://jubla.atlassian.net/wiki/spaces/WISSEN/pages/1122467867/Jubla-Datenbank#Lagererfassung-auf-der-jubla.db>`_ anschauen. Hier wird dir Schritt für Schritt erklärt, wie die Lagererfassung in der jubla.db-Datenbank funktioniert.

Lageranmeldung
==============

Generell gibt es zwei Möglichkeiten, die Lagerteilnehmer*innen auf der jubla.db anzumelden. Entweder du lässt die Anmeldung von den Teilnehmenden analog per Post ausfüllen und fügst sie anschliessend selbst in der Datenbank hinzu, oder du lässt die Anmeldung durch die Teilnehmenden oder ihren Erziehungsberechtigten selbst in der Datenbank vornehmen.

Teilnehmende als Lagerleitung hinzufügen
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In der Registerkarte ``Teilnehmende`` deines Lagers kannst du mit der Schaltfläche ``Person hinzufügen`` manuell Personen hinzufügen und ihre Rolle im Lager definieren. Wichtig ist, dass die Personen bereits ein Profil auf der jubla.db haben.

.. figure:: /media/lagerverwaltung/lageranmeldung_teilnehmende.png
    :name: 
    
    Lageranmeldung - Übersicht

Im Feld ``Person suchen`` kannst du mit dem Namen nach einer Person suchen und sie hinzufügen.

.. figure:: /media/lagerverwaltung/lageranmeldung_tn-erstellen.png
    :name: 
    
    Lageranmeldung - Teilnehmende hinzufügen

Wenn du beim Lagererstellen :ref:`Anmeldeangaben <anmeldeangaben-link-target>` und/oder :ref:`Administrationsangaben <administrationsangaben-link-target>` definiert hast, so kannst du als Nächstes die Fragen für die anzumeldende Person beantworten und unter ``Bemerkungen`` weitere relevante Informationen ergänzen. Eine Eingabeaufforderung für die ausgewählten :ref:`Kontaktangaben <kontaktangaben-link-target>` wird nicht angezeigt. Wenn du alles eingetragen hast, kannst du die Anmeldung abschliessen, indem du auf ``speichern`` drückst.

.. figure:: /media/lagerverwaltung/lageranmeldung_anmeldeangaben_ausfüllen_ll.png
    :name: 
    
    Lageranmeldung - Anmeldeangaben

In diesem :fa:`video` `Anleitungsvideo <https://jubla.atlassian.net/wiki/spaces/WISSEN/pages/1122467867/Jubla-Datenbank#Teilnehmerverwaltung-f%C3%BCrs-Lager-via-jubla.db>`_ wird dir Schritt für Schritt gezeigt, wie du die Teilnehmenden für das Lager verwalten kannst.

..  _teilnehmende_melden_sich_selbst_an-link-target:

Teilnehmende melden sich selbst an
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Die Teilnehmer*innen melden sich auf der jubla.db mit ihrem Log-in an und finden das Lager unter ``Demnächst stattfindende Anlässe`` im Modul ``Anlässe`` oder auf Ebene der Schar unter ``Lager``. Alternativ kannst du den Teilnehmer*innen auch einen :ref:`Direktlink <direktlink_bild-link-target>` zustellen.

.. figure:: /media/lagerverwaltung/lageranmeldung_lager_finden_anlaesse.png
    :name: 
    
    Lageranmeldung - über Anlässe

.. figure:: /media/lagerverwaltung/lageranmeldung_lager_finden_schar.png
    :name: 
    
    Lageranmeldung - über Schar

Durch Klicken auf ``Anmelden`` wird die Person erst aufgefordert, die :ref:`Kontaktangaben <kontaktangaben-link-target>` anzugeben und anschliessend die Fragen, welche beim Lagererstellen unter :ref:`Anmeldeangaben <anmeldeangaben-link-target>` definiert wurden, zu beantworten. Fragen unter :ref:`Administrationsangaben <administrationsangaben-link-target>` werden nicht angezeigt.

.. figure:: /media/lagerverwaltung/lageranmeldung_anmelden.png
    :name: 
    
    Lageranmeldung - Anmelden

.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_kontaktangaben.png
    :name: 
    
    Lageranmeldung - Kontaktangaben
.. figure:: /media/lagerverwaltung/lageranmeldung_anmeldeangaben_ausfüllen_tn.png
    :name: 
    
    Lageranmeldung - Anmeldeangaben

..  _lageranmeldung_elternzugang-link-target:

Lageranmeldung über den Elternzugang
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Damit die Erziehungsberechtigten/Eltern ihre Kinder selbständig auf der Datenbank anmelden können, muss deine Schar zuerst einen ``Elternzugang`` einrichten. Wie du diesen einrichten kannst, wird dir unter :ref:`Elternzugangsverwaltung <elternzugang-link-target>` erklärt. Im folgenden Abschnitt wird gezeigt, wie die Erziehungsberechtigten/Eltern anschliessend die Lageranmeldung vornehmen können.

Damit es für die Eltern möglichst einfach ist, das Lager auf der Datenbank zu finden, kannst du auf ``Direktlink kopieren`` klicken und diesen Link mit den Eltern teilen.

..  _direktlink_bild-link-target:

.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_link.png
    :name: 
    
    Lageranmeldung - Link

Wenn die Eltern den Link öffnen, landen sie direkt auf der Übersichtsseite des Lagers. Durch Klicken auf ``Anmelden`` können sie ganz einfach ihre Kinder anmelden.

.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_kind_auswahl.png
    :name: 
    
    Lageranmeldung - Anmeldung

Anschliessend können die Eltern die :ref:`Kontaktangaben <kontaktangaben-link-target>` ausfüllen und speichern. Fragen unter :ref:`Anmeldeangaben <anmeldeangaben-link-target>` und :ref:`Administrationsangaben <administrationsangaben-link-target>` werden nicht angezeigt. Die Fragen werden trotzdem auf der :ref:`Anmeldebestätigung <anmeldebestätigung-link-target>` aufgeführt und können analog beantwortet werden.

.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_anmeldebestätigung.png
    :name: 
    
    Lageranmeldung - Anmeldeangaben auf Anmeldebestätigung

.. important:: Da die Eltern nur die Kontaktangaben ausfüllen können, dürfen keine Fragen unter :ref:`Administrationsangaben <administrationsangaben-link-target>` und :ref:`Anmeldeangaben <anmeldeangaben-link-target>` auf obligatorisch gesetzt sein. Ansonsten können sie die Anmeldung nicht abschliessen.

.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_kontaktangaben.png
    :name: 
    
    Lageranmeldung - Kontaktangaben
.. figure:: /media/lagerverwaltung/lageranmeldung_elternzugang_anmeldeangaben_ausfüllen.png
    :name: 
    
    Lageranmeldung - Anmeldeangaben

In diesem :fa:`video` `Anleitungsvideo <https://jubla.atlassian.net/wiki/spaces/WISSEN/pages/1122467867/Jubla-Datenbank#Lageranmeldung-f%C3%BCr-Eltern-und-Kinder-via-jubla.db>`_ wird dir Schritt für Schritt gezeigt, wie die Eltern ihre Kinder anmelden können.

..  _anmeldebestätigung-link-target:

Anmeldebestätigung
~~~~~~~~~~~~~~~~~~~
Wenn die Lageranmeldung durch die Teilnehmenden oder durch ihre Erziehungsberechtigten ausgefüllt wird, wird nach der Anmeldung eine Anmeldebestätigung per Mail verschickt.

.. figure:: /media/lagerverwaltung/anmeldebestätigung_seite1.png
    :name: 
    
    Lageranmeldung - Anmeldebestätigung (seite 1)

.. figure:: /media/lagerverwaltung/anmeldebestätigung_seite2.png
    :name: 
    
    Lageranmeldung - Anmeldebestätigung (seite 2)
