---
unique-page-id: 9438139
description: hinzufügen Person in Blockierungsliste - Marketing Docs - Produktdokumentation
title: hinzufügen in Blockierungsliste
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# hinzufügen in Blockierungsliste {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz empfangen.

>[!NOTE]
>
>Marketo ist dabei, Begriffe wie Blacklist und Whitelist in Blockierungsliste und Zulassungsliste in unserem Produkt zu ändern. Während dieser Aktualisierung werden möglicherweise die alten Begriffe in unseren Screenshots zur Benutzeroberfläche und Dokumentation sowie die neuen Begriffe in unserem Dokumentationstext angezeigt. Wir entschuldigen uns für jede Verwirrung.

1. [Erstellen Sie ein neues Standard-Programm](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) und geben Sie ihm **Hinzufügen Namen**.
1. Klicken Sie auf **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. hinzufügen alle Personen, die Sie Ihrer **Smart-Liste** hinzufügen möchten.

   >[!NOTE]
   >
   >Personen auf Ihrer Blockierungsliste erhalten keine operativen E-Mails.

   ![](assets/three-6.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neue intelligente Kampagne**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Benennen Sie die **neue intelligente Kampagne**. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Ziehen Sie per Drag &amp; Drop **Mitglied der Smart-Liste**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Wählen Sie die eben erstellte intelligente Liste aus.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Ziehen Sie **den Datenwert**&#x200B;ändern per Drag &amp; Drop.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Geben Sie für den **Fluss** den Wert &quot; **Block Listed** &quot;für das **Attribut** ein und setzen Sie **New Value** auf **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Wählen Sie auf der Registerkarte **Plan** die Option Einmal **ausführen**.

   ![](assets/ten.png)

1. Wählen Sie **Jetzt** ausführen und klicken Sie auf **Ausführen**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Diese Personen erhalten keine E-Mails mehr.

   >[!TIP]
   >
   >Erstellen Sie eine [auslösende intelligente Kampagne](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) mit der Option &quot;Datenwert **** ändern&quot;mit der Option &quot; **Blockliste&quot;ist zukünftig für alle Personen wahr** , die über auf die Blockierungsliste setzend Attribute verfügen.

