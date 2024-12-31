---
unique-page-id: 1900579
description: Tracking für einen E-Mail-Link deaktivieren - Marketo-Dokumente - Produktdokumentation
title: Tracking für einen E-Mail-Link deaktivieren
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---

# Tracking für einen E-Mail-Link deaktivieren {#disable-tracking-for-an-email-link}

Manchmal möchten Sie die **Marketo-Tracking-URL** nicht für einen Link in einer E-Mail aktivieren. Dies ist nützlich, wenn die Zielseite URL-Parameter nicht unterstützt und zu einem fehlerhaften Link führen kann.

1. Wählen Sie Ihre E-Mail aus und klicken Sie **Entwurf bearbeiten**.

   ![](assets/one-7.png)

1. Doppelklicken Sie auf den bearbeitbaren Abschnitt, der den Link enthält.

   ![](assets/two-6.png)

1. Klicken Sie auf den betreffenden Link und dann auf die Schaltfläche **Link einfügen/bearbeiten**.

   ![](assets/three-6.png)

1. Deaktivieren Sie im Popup Link bearbeiten das Kontrollkästchen **Link nachverfolgen**.

   ![](assets/four-4.png)

1. Sie werden feststellen, dass die **Include mkt_tok-Box** verschwindet. Klicken Sie auf **Übernehmen**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Wenn Sie nur **Include mkt_tok** deaktivieren, kann der Link weiterhin verfolgt werden, aber nach der Umleitung enthält die Ziel-URL den Abfragezeichenfolgenparameter mkt_tok nicht. Dieser Parameter wird von Marketo Landingpages und Munchkin verwendet, um eine ordnungsgemäße Verfolgung von Personenaktivitäten sicherzustellen (z. B. wenn eine Person sich von einer E-Mail abmeldet). Sie sollten die Verwendung dieser Funktion vermeiden, es sei denn, Sie sehen ein seltsames Verhalten auf Ihrer Website, aufgrund des vorhandenen Parameters.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Möchten Sie das Klick-Tracking für einen Link in einer E-Mail deaktivieren **Vorlage**? Dieses Format verwenden:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Wenn Sie Hilfe bei der Implementierung benötigen, wenden Sie sich bitte an Ihren Web-Entwickler.

Schön! Sie haben jetzt das Tracking für einen Link deaktiviert.
