---
unique-page-id: 1900579
description: Deaktivieren Sie die Verfolgung für einen E-Mail-Link - Marketing Docs - Produktdokumentation
title: Deaktivieren der Verfolgung für einen E-Mail-Link
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Deaktivieren der Verfolgung für einen E-Mail-Link {#disable-tracking-for-an-email-link}

Manchmal möchten Sie die **Marketing-Tracking-URL** für einen Link in einer E-Mail nicht aktivieren. Dies ist nützlich, wenn die Zielseite keine URL-Parameter unterstützt und zu einem fehlerhaften Link führen kann.

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Bearbeiten** **Entwurf**.

   ![](assets/one-7.png)

1. Klicken Sie mit der Dublette auf den bearbeitbaren Abschnitt, der den Link enthält.

   ![](assets/two-6.png)

1. Klicken Sie auf den betreffenden Link und dann auf die Schaltfläche **Link einfügen/bearbeiten**.

   ![](assets/three-6.png)

1. Deaktivieren Sie im Popup Link bearbeiten das Kontrollkästchen **Link verfolgen**.

   ![](assets/four-4.png)

1. Beachten Sie, dass das Feld **inklusive mkt_tok** verschwindet. Klicken Sie auf **Apply**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Wenn Sie nur **inklusive mkt_tok** deaktivieren, kann der Link weiterhin verfolgt werden. Nach der Umleitung enthält die Ziel-URL jedoch nicht den Zeichenfolgenparameter &quot;mkt_tok&quot;, sondern auch nicht den Abfragen-Zeichenfolgenparameter &quot;mkt_tok&quot;. Dieser Parameter wird von Marketo-Landingpages und Munchkin verwendet, um eine ordnungsgemäße Verfolgung der Aktivitäten von Personen sicherzustellen (z. B. wenn sich ein Benutzer von einer E-Mail abmeldet). Sie sollten diese Funktion nur verwenden, wenn Sie auf Ihrer Website aufgrund des vorhandenen Parameters ein merkwürdiges Verhalten sehen.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Möchten Sie die Klick-Tracking für einen Link in einer E-Mail **template** deaktivieren? Verwenden Sie folgendes Format:
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Wenn Sie Hilfe bei der Implementierung benötigen, wenden Sie sich bitte an Ihren Webentwickler.

Schön! Sie haben jetzt die Verfolgung für einen Link deaktiviert.
