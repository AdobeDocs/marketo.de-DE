---
unique-page-id: 2949716
description: Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-In für Outlook - Marketo Docs - Produktdokumentation
title: Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-In für Outlook
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
feature: Marketo Sales Insights
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Senden und Verfolgen einer E-Mail mit dem E-Mail-Add-In für Outlook {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Sie können E-Mails mit Marketo direkt von Outlook aus senden und verfolgen.

>[!PREREQUISITES]
>
>Installieren Sie, falls noch nicht geschehen, das [Marketo-E-Mail-Add-in für Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>Die Funktionen von Sales Insight-Aktionen, einschließlich &quot;E-Mail an Vertrieb senden&quot;, &quot;Zu Vertriebskampagne hinzufügen&quot;und &quot;Aufgaben&quot;, sind nicht in den Sales Insight-E-Mail-Plugins für Gmail und Outlook verfügbar. Derzeit können Benutzer von ihrem E-Mail-Client aus nur trackbare E-Mails mit oder ohne Marketo-E-Mail-Vorlage senden, wenn sie die Sales Insight-E-Mail-Plugins verwenden.

1. Öffnen Sie Microsoft Outlook und erstellen Sie eine neue E-Mail.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Wenn Sie mehrere Empfänger in die E-Mail aufnehmen, werden alle Aktivitäten unter dem ersten Empfänger nachverfolgt.

1. Erstellen Sie Ihre E-Mail wie gewohnt und klicken Sie dann auf **Senden und Verfolgen**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Wenn Sie eine E-Mail an eine Person senden, die nicht in Ihrer Marketo-Instanz vorhanden ist, wird automatisch ein Personendatensatz für diese Benutzer erstellt. Ihr Nachname lautet immer &quot;mktUnknown&quot;, damit Sie sie leicht finden können.

   >[!TIP]
   >
   >Wenn Sie eine Marketo-Vorlage verwenden möchten, finden Sie weitere Informationen unter [Versand und Tracking aus Outlook mit einer Vorlage](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Sehen Sie sich die Vorschau an und klicken Sie auf **Senden**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >Anti-Spam-Technologie lehnt Öffnungen und Klicks, die innerhalb von 20 Sekunden nach dem Versand der E-Mail auftreten, oft ab. Warten Sie also mindestens so lange, bis Sie beim Testen geöffnet/klicken.

   Um zu sehen, wer Ihre über Outlook gesendeten E-Mails erhalten hat, erstellen Sie eine intelligente Liste mit dem Filter &quot;E-Mail zum Versand an Kunden&quot;.

   ![](assets/was-sent-sales-email.png)

So einfach ist es! Obwohl diese E-Mail von einem Outlook eines Verkäufers gesendet wurde, wird sie in Marketo verfolgt.

>[!MORELIKETHIS]
>
>[Eingehende E-Mails von Ihren Leads in Marketo anmelden](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
