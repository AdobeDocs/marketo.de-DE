---
unique-page-id: 9438139
description: hinzufügen Person in Blockierungsliste - Marketing Docs - Produktdokumentation
title: hinzufügen in Blockierungsliste
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# hinzufügen Person in Blockierungsliste {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz empfangen.

>[!NOTE]
>
>Marketo ist dabei, Begriffe wie Blacklist und Whitelist in Blockierungsliste und Zulassungsliste in unserem Produkt zu ändern. Während dieser Aktualisierung werden möglicherweise die alten Begriffe in unseren Screenshots zur Benutzeroberfläche und Dokumentation sowie die neuen Begriffe in unserem Dokumentationstext angezeigt. Wir entschuldigen uns für jede Verwirrung.

1. [Erstellen Sie ein neues Standardprogramm ](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) und nennen Sie es  **Hinzufügen Blockierungsliste**.

1. Klicken Sie auf **Neu** und wählen Sie **Neues lokales Element**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. hinzufügen Sie alle Personen, die Ihre **Smart-Liste** hinzufügen möchten, zu Ihrer Blockierungsliste hinzufügen.

   >[!NOTE]
   >
   >Personen auf Ihrer Blockierungsliste erhalten keine operativen E-Mails.

   ![](assets/three-6.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neue Smart-Kampagne**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Benennen Sie die **Neue intelligente Kampagne**. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Ziehen Sie **Mitglied der Smart-Liste** per Drag &amp; Drop.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Wählen Sie die eben erstellte intelligente Liste aus.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Ziehen Sie **Datenwert ändern** per Drag &amp; Drop.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Geben Sie für **Fluss** **Block Listed** für das **Attribut** ein und setzen Sie **Neuer Wert** auf **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Wählen Sie auf der Registerkarte **Plan** die Option **Einmal ausführen**.

   ![](assets/ten.png)

1. Wählen Sie **Jetzt ausführen** und klicken Sie auf **Ausführen**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Diese Personen erhalten keine E-Mails mehr.

   >[!TIP]
   >
   >Erstellen Sie eine intelligente Kampagne [Trigger-Blockierungsliste](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) mithilfe von **Datenwert ändern** mit **aufgelisteter  ist true** für alle zukünftig verwendbaren Personen mit Attributen, die über  verfügen.
