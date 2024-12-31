---
unique-page-id: 14352475
description: Installieren von Sales Connect-Ereignisfeldern im Aktivitätsverlauf - Marketo-Dokumente - Produktdokumentation
title: Installieren von Sales Connect-Ereignisfeldern im Aktivitätsverlauf
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 3%

---

# Installieren von Sales Connect-Ereignisfeldern im Aktivitätsverlauf {#install-sales-connect-event-fields-on-activity-history}

Nachdem Sie das Enterprise-Package in Salesforce installiert haben, können Sie Sales Connect-Ereignisfelder in Ihren Aktivitätsverlaufsabschnitt installieren. Die Felder für Sales Connect-Ereignisse enthalten Informationen wie Ansichten, Klicks und Kampagnen. Auf diese Weise können Sie Informationen zu Ihren E-Mails direkt in Salesforce importieren.

Stellen Sie bei diesen Schritten sicher, dass Sie sich mit Ihrem Salesforce-Administrator zusammentun. In diesem Beispiel installieren wir die Felder im **Lead-Seiten-Layout**. Sie können die Felder auch in die Seiten-Layouts „Kontakt“, „Konto“ und „Opportunity“ installieren. Denken Sie daran, dass Sie beim Anmelden von E-Mails an Konten und Opportunities den Kontakt, den Sie per E-Mail versenden, als Kontaktrolle benötigen.

1. Klicken Sie **Setup**.
1. Klicken Sie auf **Anpassen**.
1. Klicken Sie **Leads**.
1. Klicken Sie auf **Seiten-Layouts**.
1. Klicken Sie **Bearbeiten** neben dem Seitenlayout, das Sie ändern möchten.

   >[!NOTE]
   >
   >Sales Connect installiert einige Seiten-Layouts für Sie. Wenn Sie jedoch bereits über ein Standard-Layout verfügen, das Ihr Team verwendet, sollten Sie es dort installieren. Sie können die Sales Connect-Seiten-Layouts löschen, wenn Sie sie nicht verwenden möchten.

1. Scrollen Sie nach unten zum Abschnitt Aktivitätsverlauf .
1. Klicken Sie zum Bearbeiten auf den Schraubenschlüssel.
1. Wählen Sie die Sales Connect-Felder aus, die Sie in den Abschnitt „Aktivitätshistorie“ aufnehmen möchten. Wenn Sie hier keine Sales Connect-Felder sehen, haben Sie möglicherweise das falsche Salesforce-Paket installiert.
1. Klicken Sie **Hinzufügen**, um die gewünschten Felder zu verschieben.
1. Klicken Sie auf **OK**.
1. Klicken Sie auf **Speichern**.

   Ihre Benutzer können jetzt wertvolle Informationen und Aktualisierungen zu ihren E-Mails in Salesforce sehen!
