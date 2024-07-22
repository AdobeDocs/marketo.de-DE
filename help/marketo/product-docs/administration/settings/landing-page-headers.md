---
description: Landingpage-Kopfzeilen - Marketo-Dokumente - Produktdokumentation
title: Landingpage-Kopfzeilen
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# Landingpage-Kopfzeilen {#landing-page-headers}

Gehen Sie wie folgt vor, um einige der HTTP-Header auf Ihren Landingpage-Domänen anzupassen.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Klicken Sie auf **[!UICONTROL Landingpages]**.

   ![](assets/landing-page-headers-2.png)

1. Klicken Sie neben den Landingpage-HTTP-Headern auf **[!UICONTROL Bearbeiten]** .

   ![](assets/landing-page-headers-3.png)

1. Wählen Sie die gewünschten Einstellungen aus und klicken Sie danach auf **[!UICONTROL Speichern]** .

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Verwenden Sie dies, um sicherzustellen, dass Verbindungen zu Landingpages immer über HTTPS bereitgestellt werden (sollte nur für Abonnements mit über SSL gesicherten Landingpages festgelegt werden)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Hiermit können Sie definieren, ob gehostete Marketo Engage-Assets in externe Webseiten eingebettet werden können.</td>
 </tr>
</table>

>[!CAUTION]
>
>Es ist wichtig, diese Einstellungen zusammen mit Ihrem IT-Team zu überprüfen, um zu bestimmen, auf welche Richtlinie Ihr Unternehmen eingestellt sein soll. Falsche Einstellungen können verhindern, dass einige Besucher auf Ihre Landingpages zugreifen.
