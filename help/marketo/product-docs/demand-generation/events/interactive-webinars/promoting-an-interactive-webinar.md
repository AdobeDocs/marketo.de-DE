---
description: Weiterleiten eines interaktiven Webinars - Marketo-Dokumente - Produktdokumentation
title: Weiterleiten eines interaktiven Webinars
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 6747a7b85047024d295ecc2c061bb6370ccfe0b9
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Weiterleiten eines interaktiven Webinars {#promoting-an-interactive-webinar}

Die Weiterleitung eines interaktiven Webinars ähnelt der Weiterleitung eines Partner-Webinars über Launchpoint. Bei der Erstellung eines Ereignisprogramms für ein interaktives Webinar können Sie Mitglieder hinzufügen, indem Sie eine Kampagne ausführen oder Mitglieder zum Programm importieren. Um die Mitglieder zu überprüfen, die zum Ereignisprogramm für interaktive Webinare hinzugefügt wurden, klicken Sie auf die Registerkarte **Mitglieder** .

![](assets/promoting-an-interactive-webinar-1.png)

Nachdem die Mitglieder hinzugefügt oder importiert wurden, können Sie im interaktiven Webinar-Veranstaltungsprogramm eine E-Mail-Kampagne erstellen, um eine Einladung an alle Programmmitglieder zu senden und deren Status nach dem Versand der E-Mail auf &quot;eingeladen&quot;zu ändern.

>[!NOTE]
>
>Wenn Sie dem interaktiven Webinar-Veranstaltungsprogramm einen Mitwirt oder einen Moderator als Zielgruppenmitglied hinzufügen möchten, müssen Sie für diese eine andere E-Mail-ID verwenden. Andernfalls wird ihnen der Fehler &quot;Diese E-Mail ist bereits registriert&quot;angezeigt.

Die E-Mail kann spezifische Programmdetails enthalten sowie eine Landingpage-URL enthalten, über die der Empfänger zu einer bestimmten Seite weitergeleitet wird, auf der weitere Informationen zum Webinar (z. B. Inhalt, Moderatorinformationen usw.) hinzugefügt werden können. Diese Landingpage kann als lokales Asset im interaktiven Webinar-Veranstaltungsprogramm erstellt werden.

Sie können eine Registrierung für dieses Webinar anfordern, indem Sie ein Formular auf der Landingpage aktivieren und die Formularklicks mit der aktivierten Registrierung im interaktiven Webinar Event Program verknüpfen. Anschließend kann eine Kampagne erstellt werden, die Formularübermittlungen als Trigger verwendet und den Programmstatus von &quot;eingeladen&quot;in &quot;registriert&quot;ändert.

>[!NOTE]
>
>Der Übergang von &quot;eingeladen&quot;zu &quot;registriert&quot;erfolgt nicht automatisch in interaktiven Webinaren, da es mehrere Trigger geben kann, die die Transition erstellen.

Sobald ein Mitglied in einem interaktiven Webinar-Veranstaltungsprogramm im &quot;registrierten&quot;Programmstatus war, wird automatisch eine Registrierung für das in Adobe Connect erstellte Webinar vorgenommen. Registrierungsdaten wie Vorname, Nachname und E-Mail-ID werden dann an Adobe Connect übertragen. Das bedeutet, dass die Informationen dem Moderator oder dem Gastgeber während des Webinars zur Verfügung stehen, sobald der Nutzer als Teilnehmer am Webinar teilnimmt.

Innerhalb weniger Minuten nach der Registrierung wird die Webinar-URL für das Mitglied auf der Registerkarte Mitglieder ausgefüllt. Wenn Sie die Spalte für die Webinar-URL nicht finden können, stellen Sie sicher, dass die Spalte zu Ihrer Ansicht hinzugefügt wurde. Dies ist eine personalisierte URL für jedes registrierte Mitglied, damit es zum geplanten Zeitpunkt in das Webinar eintreten kann, ohne dass eine Authentifizierung erforderlich ist. Intern ausgetauschte Token kümmern sich um die Authentifizierung der Mitglieder.

Mit dem `{{member.webinar url}}` [Token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} können Sie die Webinar-URL für einzelne Mitglieder einer E-Mail-Kampagne einbeziehen, um mitzuteilen, dass sie in dem Ereignis registriert wurden, und um über die Anschließungs-URL zum geplanten Zeitpunkt in das Webinar zu gelangen. Kalendertoken können in derselben E-Mail-Kampagne verwendet werden, um sicherzustellen, dass der Webinarplan den Kalender der Mitglieder hinzugefügt werden kann.

Links zum Erstellen einer Landingpage und einer E-Mail-Kampagne finden Sie auf der rechten Seite des Tabs Übersicht Ihres Veranstaltungsprogramms. Die übrigen Promotions, die sich auf eine Veranstaltung beziehen, bleiben mit den Partner-Webinaren identisch, die die Launchpoint-Integration verwenden.

![](assets/promoting-an-interactive-webinar-2.png)

Mit interaktiven Webinaren können Sie eine Registrierung vor, während oder nach einem Webinar anfordern. In allen Fällen müssen Sie einfach die Webinar-URL für den Lead freigeben. Wenn Sie auf den Link klicken, bevor das Webinar beginnt, werden diese an eine Pre-Webinar-Landingpage gesendet. Wenn Sie im Webinar darauf klicken, gelangen die Benutzer zum laufenden Webinar. Wenn Sie darauf klicken, nachdem das Webinar das Video aufgenommen hat, gelangen Sie zu einer Aufzeichnung des Webinars.

## Interaktive Webinare-Token {#interactive-webinars-tokens}

Verwenden Sie Token, um interaktive Webinare in E-Mails und Landingpages zu bewerben, ohne manuell Webinardetails hinzufügen zu müssen. Dadurch wird die Gesamteffizienz verbessert, da Änderungen an den Webinar-Metadaten (z. B. Webinartitel, Startdatum usw.) automatisch in Ihren Assets übernommen werden.

![](assets/promoting-an-interactive-webinar-3.png)

**Liste der Token**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle
