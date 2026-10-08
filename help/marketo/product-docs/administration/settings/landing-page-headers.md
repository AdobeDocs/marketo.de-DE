---
description: Anpassen von HTTP-Kopfzeilen für Landingpage-Domains, einschließlich der Optionen Strict-Transport-Security und X-Frame-Options.
title: Header der Landingpage
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: 'https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 4%
---
# Header der Landingpage {#landing-page-headers}

Gehen Sie wie folgt vor, um einige HTTP-Kopfzeilen in den Domains Ihrer Landingpage anzupassen.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Klicken Sie auf **[!UICONTROL Landingpages]**.

   ![](assets/landing-page-headers-2.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** neben Landingpage-HTTP-Kopfzeilen.

   ![](assets/landing-page-headers-3.png)

1. Wählen Sie die gewünschten Einstellungen aus und klicken Sie **[!UICONTROL auf &quot;]**&quot;.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Hiermit können Sie garantieren, dass Verbindungen zu Landingpages immer über HTTPS bereitgestellt werden (sollte nur für Abonnements mit durch SSL gesicherten Landingpages festgelegt werden).</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Ermöglicht die Definition, ob in Marketo Engage gehostete Assets in externe Webseiten eingebettet werden können</td>
 </tr>
</table>

>[!CAUTION]
>
>Es ist wichtig, diese Einstellungen mit Ihrem IT-Team zu überprüfen, um zu bestimmen, auf welche Richtlinie Ihre Organisation eingestellt werden soll. Falsche Einstellungen können dazu führen, dass einige Besucher nicht auf Ihre Landingpages zugreifen können.
