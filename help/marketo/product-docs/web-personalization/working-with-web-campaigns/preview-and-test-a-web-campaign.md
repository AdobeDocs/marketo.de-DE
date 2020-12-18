---
unique-page-id: 10092925
description: Vorschau und Testen einer Web-Kampagne - Marketing Docs - Produktdokumentation
title: Vorschau und Testen einer Web-Kampagne
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Vorschau und Testen einer Web-Kampagne {#preview-and-test-a-web-campaign}

Dieser Artikel zeigt Ihnen verschiedene Möglichkeiten zur Vorschau einer Web-Kampagne und zum Testen der  mithilfe eines Sandbox-Segments live auf Ihrer Website.

## Vorschau einer Web-Kampagne auf der Erstellungsseite {#preview-a-web-campaign-on-the-creation-page}

1. Gehen Sie zu **Web** **Kampagnen**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Klicken Sie auf** Neue Web-Kampagne erstellen**** **oder auf das Symbol, um eine bestehende Kampagne zu bearbeiten.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Fügen Sie in der Vorschau auf der Site die Seiten-URL hinzu und klicken Sie auf **Vorschau**. Ein neues Fenster/eine neue Registerkarte mit der Vorschau der Kampagne wird geöffnet.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Klicken Sie auf **Freigeben**, um eine E-Mail mit einer festen URL der Vorschau &quot;Kampagne&quot;zu öffnen.

   >[!NOTE]
   >
   >Sie haben auch die Möglichkeit, ein Browser-Plugin zu installieren (entweder [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) oder [Firefox](http://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi)), um eine Vorschau Ihrer Kampagne zu erhalten. Siehe den Abschnitt unten.

## Vorschau einer Web-Kampagne auf der Erstellungsseite mithilfe des Browser-Plugins {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Führen Sie die Schritte 1 und 2 von `section above` aus.
1. Klicken Sie auf den Link zum Browser-Plugin (in diesem Fall verwenden wir Chrome).

   ![](assets/4-1.png)

1. Ein neues Fenster/eine neue Registerkarte wird geöffnet. Klicken Sie auf **Hinzufügen auf Chrome**.

   ![](assets/five.png)

1. Klicken Sie auf **Hinzufügen Extension**.

   ![](assets/six.png)

1. Geh zurück nach Marketo. hinzufügen Sie die Seiten-URL und klicken Sie auf **Vorschau**.

   ![](assets/seven.png)

1. Es wird ein neues Fenster/eine neue Registerkarte geöffnet, in dem Sie die Vorschau des Aussehens Ihrer Kampagne auf einem Desktop-, Smartphone- oder Tablet-Computer festlegen können.

   ![](assets/campaign-preview.png)

## Vorschau einer Web-Kampagne auf der Webseite der Web-Kampagnen {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Wählen Sie beim Betrachten der Liste Ihrer Web-Kampagnen einfach eine Kampagne aus und klicken Sie auf das Symbol **Vorschau**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Einfach!

## Vorschau einer Web-Kampagne auf Ihrer Website {#preview-a-web-campaign-on-your-website}

Erstellen Sie ein Sandbox-Segment und eine Kampagne.

1. Gehen Sie zu **Segmente**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Klicken Sie auf **Neu erstellen**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Benennen Sie das Segment.
1. Ziehen Sie unter &quot;Verhalten&quot;Seiten einschließen auf die Arbeitsfläche. hinzufügen Sie den Wert *sandbox=1*. Klicken Sie auf Kampagne speichern und definieren.

   ![](assets/segment.png)

1. Ändern Sie auf der Seite &quot;Web-Kampagne festlegen&quot;das Segmentsegment der Zielgruppe in das Sandbox-Segment, indem Sie es aus der Liste auswählen.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Füllen Sie die Kampagne kreativ aus und klicken Sie auf **Starten**.\
   ![](assets/click-launch.jpg)

1. Gehen Sie zu Ihrer Website und fügen Sie den URL-Parameter &quot;?sandbox=1&quot;am Ende der URL hinzu. Beispiel: [www.marketo.com?sandbox=1](http://www.marketo.com/?sandbox=1)
1. Sehen Sie sich die Kampagne reagieren auf Ihrer Website.

>[!NOTE]
>
>Kampagnen reagieren nur einmal während eines Besuchers. Um die Kampagne erneut anzuzeigen, löschen Sie die Browsercookies.

>[!NOTE]
>
>Umgeleitete Kampagnen können nicht in der Vorschau angezeigt werden. Die einzige Möglichkeit, sie zu testen, ist die Verwendung eines Sandbox-Segments (das nach bestimmten Zielgruppen - *sandbox=redirect*))

