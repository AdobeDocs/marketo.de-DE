---
unique-page-id: 2949716
description: Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-in  [!DNL Outlook]  Marketo-Dokumente - Produktdokumentation
title: Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-in für  [!DNL Outlook]
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-in für [!DNL Outlook] {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Sie können E-Mails mit Marketo direkt von [!DNL Outlook] aus senden und verfolgen.

>[!PREREQUISITES]
>
>Wenn Sie dies noch nicht getan haben, installieren Sie das Add-in [Marketo-E-Mail für [!DNL Outlook]](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>Die Aktionsfunktionen von Sales Insight, einschließlich „Verkaufs-E-Mail senden“, „Zu Verkaufskampagne hinzufügen“ und „Aufgaben“, sind in den E-Mail-Plug-ins von Sales Insight für Gmail und Outlook nicht verfügbar. Derzeit haben Benutzer nur die Möglichkeit, über ihren E-Mail-Client eine verfolgbare E-Mail mit oder ohne Marketo-E-Mail-Vorlage zu senden, wenn sie die E-Mail-Plug-ins für Sales Insight verwenden.

1. Öffnen Sie Microsoft Outlook und erstellen Sie eine neue E-Mail.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Wenn Sie mehrere Empfänger in die E-Mail einbeziehen, wird jede Aktivität unter dem ersten Empfänger verfolgt.

1. Erstellen Sie Ihre E-Mail wie gewohnt und klicken Sie dann auf **[!UICONTROL Senden und Verfolgen]**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Wenn Sie eine E-Mail an eine Person senden, die nicht in Ihrer Marketo-Instanz vorhanden ist, wird automatisch ein Personendatensatz für diese Person erstellt. Ihr Nachname lautet immer „mktUnknown“, damit Sie sie leicht finden können.

   >[!TIP]
   >
   >Wenn Sie eine Marketo-Vorlage verwenden möchten, lesen Sie [Senden und Verfolgen von [!DNL Outlook] Verwenden einer Vorlage](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Sehen Sie sich die Vorschau an und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >Die Anti-Spam-Technologie lehnt häufig Öffnungen und Klicks ab, die innerhalb von 20 Sekunden nach dem Versand der E-Mail auftreten. Warten Sie also beim Testen mindestens so lange, bis sie geöffnet/geklickt hat.

   Um zu sehen, wer Ihre E-Mails über [!DNL Outlook] erhalten hat, erstellen Sie eine Smart-Liste mit dem Filter &quot;[!UICONTROL Wurde gesendet Verkaufs-E-Mail]&quot;.

   ![](assets/was-sent-sales-email.png)

So einfach ist das! Obwohl diese E-Mail vom [!DNL Outlook] eines Vertriebsmitarbeiters gesendet wurde, wird sie in Marketo verfolgt.

>[!MORELIKETHIS]
>
>[Eingehende E-Mails von Ihren Leads in Marketo protokollieren](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
