Anhang 2: MailChimp
===================

Mit dem MailChimp-Export können die EmpfängerInnen von Mailinglisten in
eine MailChimp-Liste exportiert werden.

.. caution:: Die MailChimp-Liste wird durch den Export **überschrieben**, d.h. EmpfängerInnen, welche in Hitobito der zu exportierenden Liste nicht mehr angehören (weil sie z.B. die entsprechende Rolle nicht mehr haben), werden in MailChimp beim nächsten Export gelöscht.

.. hint:: Die MailChimp-Liste wird nur auf Knopfdruck exportiert und nicht periodisch, d.h. vor jedem E-Mailversand sollte ein Export ausgelöst werden.

Das MailChimp-Feature ermöglicht es, die in hitobito organisierten Daten zu brauchen, um mit MailChimp gestaltete Newsletter zu versenden. Es kann nicht gebraucht werden, um eine MailChimp-Liste mit einer hitobito-Mailingliste zu synchronisieren, da es keine Daten von MailChimp importiert und bestehende Daten von MailChimp bei jedem Export löscht.

Verknüpfen einer Mailingliste mit MailChimp
-------------------------------------------

Mit jeder Mailingliste kann jeweils eine MailChimp-Audience verknüpft werden. Dies geschieht in den Einstellungen der Mailingliste durch die beiden Felder «MailChimp API-Schlüssel» und «MailChimp Listen-ID»:

.. image:: media/Liste_Info-Mailchimp.png

.. hint:: Standardmässig werden nur die Haupt-E-Mailadressen der Abonnent*innen synchronisiert. Sollen weitere E-Mailadressen, welche die Option "Versand" haben ebenfalls mit MailChimp synchronisiert werden, ist die Option "Alle Versandadressen synchronisieren" anzuwählen.

Die «MailChimp Listen-ID» können Sie in den Einstellungen der gewünschten Audience in MailChimp holen (in gelb oben rechts):

 .. image:: /media/image58.png

Der «MailChimp API-Schlüssel» ermöglicht es einer fremden Applikation wie hitobito, in Ihrem Namen Änderungen in MailChimp vorzunehmen. Sie können einen neuen API-Schlüssel im Menu «Extras / API keys» in den Einstellungen Ihres Profils erstellen. Auf der entsprechenden Seite können Sie «Create A Key» drücken (im Bild unten links) und den «API key» aus dem Textfeld (im Bild gelb hinterlegt) in das entsprechende Feld in hitobito kopieren:

 .. image:: media/image59.png

Gratuliere, nach dem Speichern dieser zwei Informationen ist nun Ihre Mailingliste mit der MailChimp-Liste verknüpft!

Exportieren nach MailChimp
--------------------------

Um die EmpfängerInnen einer Mailingliste nach MailChimp zu exportieren, wählen Sie die entsprechende Option unter «Export» in der Ansicht «Abonnenten» Ihrer Mailingliste in hitobito aus:

.. image:: /media/image60.png

Nach dem Auslösen des Exports wird die Liste im Hintergrund in die gewählte MailChimp-Audience exportiert und die EmpfängerInnen Ihrer Mailingliste sollten nach kurzer Zeit dort erscheinen.

.. note:: EmpfängerInnen Ihrer Mailingliste, welche sich in der Vergangenheit aktiv bei MailChimp von Ihrer Liste abgemeldet haben (über den Abmelden-Link in Ihrer E-Mail), behalten ihren «Unsubscribed»-Status und erhalten auch nach einem neuerlichen Export aus hitobito keine E-Mails mehr von Ihnen.
