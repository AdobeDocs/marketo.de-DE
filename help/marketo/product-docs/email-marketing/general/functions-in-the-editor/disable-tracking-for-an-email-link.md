---
unique-page-id: 1900579
description: Tracking für einen E-Mail-Link deaktivieren - Marketo-Dokumente - Produktdokumentation
title: Tracking für einen E-Mail-Link deaktivieren
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Tracking für einen E-Mail-Link deaktivieren {#disable-tracking-for-an-email-link}

Manchmal möchten Sie die **Marketo Tracking URL** auf einen Link in einer E-Mail klicken. Dies ist nützlich, wenn die Zielseite URL-Parameter nicht unterstützt und zu einem fehlerhaften Link führen kann.

1. E-Mail auswählen und auf **Entwurf bearbeiten**.

   ![](assets/one-7.png)

1. Doppelklicken Sie auf den bearbeitbaren Abschnitt, der den Link enthält.

   ![](assets/two-6.png)

1. Klicken Sie auf den entsprechenden Link und anschließend auf die Schaltfläche **Link einfügen/bearbeiten** Schaltfläche.

   ![](assets/three-6.png)

1. Deaktivieren Sie im Popup Link bearbeiten die Option **Link verfolgen** aktivieren.

   ![](assets/four-4.png)

1. Sie werden die **mkt_tok-Feld einschließen** verschwindet. Klicks **Anwenden**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Deaktivieren von **mkt_tok einschließen** lässt weiterhin zu, dass der Link verfolgt wird, aber nach einer Umleitung enthält die Ziel-URL nicht den Abfragezeichenfolgenparameter mkt_tok . Dieser Parameter wird von Marketo-Einstiegsseiten und Munchkin verwendet, um eine ordnungsgemäße Verfolgung der Personenaktivitäten sicherzustellen (z. B. wenn sich eine Person von einer E-Mail abmeldet). Sie sollten die Verwendung dieser Funktion vermeiden, es sei denn, Sie sehen auf Ihrer Website ein seltsames Verhalten aufgrund des vorhandenen Parameters.

1. Klicks **Speichern**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Möchten Sie das Klick-Tracking für einen Link in einer E-Mail deaktivieren **template**? Verwenden Sie dieses Format:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Wenden Sie sich an Ihren Web-Entwickler, wenn Sie Hilfe bei der Implementierung benötigen.

Gut! Sie haben nun das Tracking für einen Link deaktiviert.
