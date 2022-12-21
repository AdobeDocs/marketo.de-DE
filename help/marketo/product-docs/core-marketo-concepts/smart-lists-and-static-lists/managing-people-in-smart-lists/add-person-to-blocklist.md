---
unique-page-id: 9438139
description: Person zu Blockierungsliste hinzufügen - Marketo Docs - Produktdokumentation
title: Person zu Blockierungsliste hinzufügen
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Person zu Blockierungsliste hinzufügen {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz erhalten.

>[!NOTE]
>
>Marketo ist dabei, Begriffe wie Blacklist und Whitelist zu Blockierungsliste und Zulassungsliste in unserem Produkt zu ändern. Während dieser Aktualisierung werden möglicherweise die alten Begriffe in unseren Screenshots der Benutzeroberfläche und Dokumentation sowie die neuen Begriffe in unserem Dokumentationstext angezeigt. Wir entschuldigen uns für jede Verwirrung.

1. [Neues Standardprogramm erstellen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) und benennen Sie sie **Zu Blockierungsliste hinzufügen**.

1. Klicken **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Fügen Sie alle Personen zu Ihren **Smart List** Sie möchten zu Ihrer Blockierungsliste hinzugefügt werden.

   >[!NOTE]
   >
   >Personen auf Ihrer Blockierungsliste erhalten keine operativen E-Mails.

   ![](assets/three-6.png)

1. Klicken **Neu** und wählen Sie **Neue intelligente Kampagne**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Benennen Sie die **Neue intelligente Kampagne**. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Drag &amp; Drop **Mitglied der Smart List**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Wählen Sie die soeben erstellte Smart-Liste aus.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Drag &amp; Drop **Datenwert ändern**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Für **Fluss**, eingeben **Block Listed** für **Attribut** und **Neuer Wert** nach **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Im **Zeitplan** Registerkarte, wählen Sie **Einmal ausführen**.

   ![](assets/ten.png)

1. Auswählen **Jetzt ausführen** und klicken Sie auf **Ausführen**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   JA! Diese Personen erhalten keine E-Mails mehr.

   >[!TIP]
   >
   >Erstellen Sie eine [Smart-Kampagne für Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) using **Datenwert ändern** mit **Block Listed is true** für alle zukünftigen Personen mit Attributen, die über Blockierungsliste verfügen.
