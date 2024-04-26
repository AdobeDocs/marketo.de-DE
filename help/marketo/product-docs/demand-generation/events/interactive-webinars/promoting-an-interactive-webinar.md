---
description: Weiterleiten eines interaktiven Webinars - Marketo-Dokumente - Produktdokumentation
title: Weiterleiten eines interaktiven Webinars
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 7f90ff09fbab7bc1559ce75b213cb86bd3cd25f4
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Weiterleiten eines interaktiven Webinars {#promoting-an-interactive-webinar}

Die Weiterleitung eines interaktiven Webinars ähnelt der Weiterleitung eines Partner-Webinars über Launchpoint. Bei der Erstellung eines Ereignisprogramms für ein interaktives Webinar können Sie einem Programm Mitglieder hinzufügen, indem Sie entweder eine Kampagne durchführen oder Mitglieder zum Programm importieren. Um die Mitglieder zu überprüfen, die zum Ereignisprogramm für interaktive Webinare hinzugefügt wurden, klicken Sie auf die Registerkarte Mitglieder .

![](assets/promoting-an-interactive-webinar-1.png)

Nachdem die Mitglieder hinzugefügt oder in das Programm importiert wurden, können Sie innerhalb des Interaktiven Webinar-Veranstaltungsprogramms eine E-Mail-Kampagne erstellen, um eine Einladung an alle Programmmitglieder zu senden und deren Status nach dem Versand der E-Mail als &quot;eingeladen&quot;zu ändern.

Die E-Mail kann spezifische Programmdetails enthalten sowie eine Landingpage-URL enthalten, über die der Empfänger zu einer bestimmten Seite weitergeleitet wird, auf der weitere Informationen zum Webinar verfügbar sind (z. B. Inhalt, Moderatorinformationen usw.) hinzugefügt werden. Diese Landingpage kann als lokales Asset im interaktiven Webinar-Veranstaltungsprogramm erstellt werden.

Sie können eine Registrierung für dieses Webinar anfordern, indem Sie ein Formular auf der Landingpage aktivieren und die Formularklicks mit der aktivierten Registrierung im interaktiven Webinar Event Program verknüpfen. Anschließend kann eine Kampagne erstellt werden, die Formularübermittlungen als Trigger verwendet und den Programmstatus von &quot;eingeladen&quot;in &quot;registriert&quot;ändert.

>[!NOTE]
>
>Der Übergang von &quot;eingeladen&quot;zu &quot;registriert&quot;erfolgt nicht automatisch in interaktiven Webinaren, da es mehrere Trigger geben kann, die die Transition erstellen.

Sobald ein Mitglied in einem interaktiven Webinar-Veranstaltungsprogramm im &quot;registrierten&quot;Programmstatus war, wird automatisch eine Registrierung für das in Adobe Connect erstellte Webinar vorgenommen. Registrierungsdaten wie Vorname, Nachname und E-Mail-ID werden dann an Adobe Connect übertragen. Das bedeutet, dass die Informationen dem Moderator oder dem Gastgeber während des Webinars zur Verfügung stehen, sobald der Nutzer als Teilnehmer am Webinar teilnimmt.

Innerhalb weniger Minuten nach der Registrierung wird die Webinar-URL für das Mitglied auf der Registerkarte Mitglieder ausgefüllt. Wenn Sie die Spalte für die Webinar-URL nicht finden können, stellen Sie sicher, dass die Spalte zu Ihrer Ansicht hinzugefügt wurde. Dies ist eine personalisierte URL für jedes registrierte Mitglied, damit es zum geplanten Zeitpunkt in das Webinar eintreten kann, ohne dass eine Authentifizierung erforderlich ist. Intern ausgetauschte Token kümmern sich um die Authentifizierung der Mitglieder.

Sie können Token verwenden, um die Webinar-URL für einzelne Mitglieder einer E-Mail-Kampagne einzubeziehen, um mitzuteilen, dass sie bei der Veranstaltung registriert wurden, und um über die Join-URL zum geplanten Zeitpunkt in das Webinar zu gelangen. Kalendertoken können in derselben E-Mail-Kampagne verwendet werden, um sicherzustellen, dass der Webinarplan den Kalender der Mitglieder hinzugefügt werden kann.

Links zum Erstellen einer Landingpage und einer E-Mail-Kampagne finden Sie auf der rechten Seite des Tabs Übersicht Ihres Veranstaltungsprogramms. Die übrigen Promotions, die sich auf eine Veranstaltung beziehen, bleiben mit den Partner-Webinaren identisch, die die Launchpoint-Integration verwenden.

![](assets/promoting-an-interactive-webinar-2.png)

Mit interaktiven Webinaren können Sie eine Registrierung vor, während oder nach einem Webinar anfordern. In allen Fällen müssen Sie einfach die Webinar-URL für den Lead freigeben. Wenn Sie auf den Link klicken, bevor das Webinar beginnt, werden diese an eine Pre-Webinar-Landingpage gesendet. Wenn Sie im Webinar darauf klicken, gelangen die Benutzer zum laufenden Webinar. Wenn Sie darauf klicken, nachdem das Webinar das Video aufgenommen hat, gelangen Sie zu einer Aufzeichnung des Webinars.
