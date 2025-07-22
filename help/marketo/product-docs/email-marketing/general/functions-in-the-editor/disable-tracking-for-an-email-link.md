---
unique-page-id: 1900579
description: Tracking für einen E-Mail-Link deaktivieren - Marketo-Dokumente - Produktdokumentation
title: Tracking für einen E-Mail-Link deaktivieren
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Tracking für einen E-Mail-Link deaktivieren {#disable-tracking-for-an-email-link}

Manchmal möchten Sie die **Marketo-Tracking-URL** nicht für einen Link in einer E-Mail aktivieren. Dies ist nützlich, wenn die Zielseite URL-Parameter nicht unterstützt und zu einem fehlerhaften Link führen kann.

Wenn eine E-Mail vor mehr als 365 Tagen gesendet wurde **und** niemand in den letzten 180 Tagen auf einen ihrer Links geklickt hat, bereinigt Marketo Engage die Route zur URL aus unserer Datenbank, was dazu führt, dass der Link unterbrochen wird. Wenn der Link also dauerhaft sein soll, sollten Sie das Tracking deaktivieren.

1. Wählen Sie Ihre E-Mail aus und klicken Sie **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/one-7.png)

1. Doppelklicken Sie auf den bearbeitbaren Abschnitt, der den Link enthält.

   ![](assets/two-6.png)

1. Klicken Sie auf den betreffenden Link und dann auf die Schaltfläche **Link einfügen/bearbeiten**.

   ![](assets/three-6.png)

1. Deaktivieren Sie im Popup Link bearbeiten das Kontrollkästchen **[!UICONTROL Link nachverfolgen]**.

   ![](assets/four-4.png)

1. Sie werden feststellen, dass das **[!UICONTROL Include mkt_tok]-Feld** verschwindet. Klicken Sie auf **[!UICONTROL Übernehmen]**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Wenn Sie nur **Include mkt_tok** deaktivieren, kann der Link weiterhin verfolgt werden, aber nach der Umleitung enthält die Ziel-URL den Abfragezeichenfolgenparameter mkt_tok nicht. Dieser Parameter wird von Marketo Landingpages und Munchkin verwendet, um eine ordnungsgemäße Verfolgung von Personenaktivitäten sicherzustellen (z. B. wenn eine Person sich von einer E-Mail abmeldet). Sie sollten die Verwendung dieser Funktion vermeiden, es sei denn, Sie sehen ein seltsames Verhalten auf Ihrer Website, aufgrund des vorhandenen Parameters.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >Wenn Sie das Klick-Tracking für einen Link in einer E-Mail-Vorlage oder die [Textversion](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"} einer E-Mail deaktivieren möchten, fügen Sie die `mktNoTrack` am *Anfang* der Zeichenfolge hinzu, nicht am Ende, wie in diesem Beispiel: `<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`. Andernfalls könnte dies dazu führen, dass der Link ausgeblendet wird. Wenn Sie Hilfe bei der Implementierung des obigen Codes benötigen, wenden Sie sich an Ihren Web-Entwickler.
