---
description: Landingpage-Kopfzeilen - Marketo-Dokumente - Produktdokumentation
title: Landingpage-Kopfzeilen
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
source-git-commit: a3acf82afa894160b20dff76fdd5132a234dfbd3
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 2%

---

# Landingpage-Kopfzeilen {#landing-page-headers}

Gehen Sie wie folgt vor, um einige der HTTP-Header auf Ihren Landingpage-Domänen anzupassen.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/landing-page-headers-1.png)

1. Klicken Sie auf **Landing Pages**.

   ![](assets/landing-page-headers-2.png)

1. Klicken **Bearbeiten** neben Landingpage-HTTP-Kopfzeilen.

   ![](assets/landing-page-headers-3.png)

1. Wählen Sie Ihre gewünschten Einstellungen aus und klicken Sie auf **Speichern** wann geschehen.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Verwenden Sie dies, um sicherzustellen, dass Verbindungen zu Landingpages immer über HTTPS bereitgestellt werden (sollte nur für Abonnements mit über SSL gesicherten Landingpages festgelegt werden)</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>Hiermit können Sie definieren, ob gehostete Marketo Engage-Assets in externe Webseiten eingebettet werden können.</td>
 </tr>
</table>

>[!CAUTION]
>
>Es ist wichtig, diese Einstellungen zusammen mit Ihrem IT-Team zu überprüfen, um zu bestimmen, auf welche Richtlinie Ihr Unternehmen eingestellt sein soll. Falsche Einstellungen können verhindern, dass einige Besucher auf Ihre Landingpages zugreifen.
