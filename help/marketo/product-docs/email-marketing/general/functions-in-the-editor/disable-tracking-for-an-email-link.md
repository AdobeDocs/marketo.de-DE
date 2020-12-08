---
unique-page-id: 1900579
description: Deaktivieren Sie die Verfolgung für einen E-Mail-Link - Marketing Docs - Produktdokumentation
title: Deaktivieren der Verfolgung für einen E-Mail-Link
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---


# Deaktivieren der Verfolgung für einen E-Mail-Link {#disable-tracking-for-an-email-link}

Manchmal möchten Sie die **Marketing-Tracking-URL** nicht auf einem Link in einer E-Mail aktivieren. Dies ist nützlich, wenn die Zielseite keine URL-Parameter unterstützt und zu einem fehlerhaften Link führen kann.

>[!NOTE]
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](/help/marketo/getting-started/updates-to-marketo-terminology.md).

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Bearbeiten** des **Entwurfs**.

   ![](assets/one-7.png)

1. Klicken Sie mit der Dublette auf den bearbeitbaren Abschnitt, der den Link enthält.

   ![](assets/two-6.png)

1. Klicken Sie auf den betreffenden Link und dann auf die Schaltfläche **Link** einfügen/bearbeiten.

   ![](assets/three-6.png)

1. Deaktivieren Sie im Popup &quot;Link bearbeiten&quot;das Kontrollkästchen &quot;Link **verfolgen&quot;** .

   ![](assets/four-4.png)

1. Sie werden feststellen, dass das Feld **Include mkt_tok nicht mehr angezeigt wird** . Klicken Sie auf **Übernehmen**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Wenn Sie die Option **Nur mkt_tok** einschließen deaktivieren, kann der Link weiterhin verfolgt werden, aber nach der Umleitung enthält die Ziel-URL nicht den Zeichenfolgenparameter mkt_tok für die Abfrage. Dieser Parameter wird von Marketo-Landingpages und Munchkin verwendet, um eine ordnungsgemäße Verfolgung der Aktivitäten von Personen sicherzustellen (z. B. wenn sich ein Benutzer von einer E-Mail abmeldet). Sie sollten diese Funktion nur verwenden, wenn Sie auf Ihrer Website aufgrund des vorhandenen Parameters ein merkwürdiges Verhalten sehen.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Möchten Sie die Klick-Tracking für einen Link in einer E-Mail- **Vorlage**deaktivieren? Verwenden Sie folgendes Format:
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Wenn Sie Hilfe bei der Implementierung benötigen, wenden Sie sich bitte an Ihren Webentwickler.

Schön! Sie haben jetzt die Verfolgung für einen Link deaktiviert.
