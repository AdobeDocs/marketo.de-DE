---
unique-page-id: 10092925
description: Vorschau und Testen einer Web-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Vorschau und Test einer Web-Kampagne
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 1%

---

# Vorschau und Test einer Web-Kampagne {#preview-and-test-a-web-campaign}

Dieser Artikel zeigt Ihnen verschiedene Möglichkeiten, eine Web-Kampagne in der Vorschau anzuzeigen und sie mit einem Sandbox-Segment live auf Ihrer Website zu testen.

>[!NOTE]
>
>Die Vorschau zeigt nur, wie die Kampagne auf der ausgewählten Website aussehen wird. Links und Widgets funktionieren nicht, da fehlerhafte Klicks/Ansichten in der Analyse vermieden werden.

## Vorschau einer Web-Kampagne auf der Erstellungsseite {#preview-a-web-campaign-on-the-creation-page}

1. Gehen Sie zu **Web-Kampagnen**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Klicken Sie **Neue Web-Kampagne erstellen** oder auf das Symbol, um eine vorhandene Kampagne zu bearbeiten.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Fügen Sie in der Vorschau auf der Site die Seiten-URL hinzu und klicken Sie auf **Vorschau**. Ein neues Fenster/eine neue Registerkarte wird mit der Kampagnenvorschau geöffnet.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Klicken Sie **Freigeben**, um eine E-Mail mit einer festen URL der Kampagnenvorschau zu öffnen.

   >[!NOTE]
   >
   >Sie haben außerdem die Möglichkeit, ein Browser-Plug-in (entweder [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) oder [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) zu installieren, um eine optimale Vorschau Ihrer Kampagne zu erhalten. Siehe folgenden Abschnitt.

## Vorschau einer Web-Kampagne auf der Erstellungsseite mithilfe des Browser-Plug-ins {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Führen Sie die Schritte 1 und 2 aus dem obigen Abschnitt aus.

1. Klicken Sie auf den Link zum Browser-Plug-in (in diesem Fall verwenden wir Chrome).

   ![](assets/4-1.png)

1. Ein neues Fenster/eine neue Registerkarte wird geöffnet. Klicken Sie **Zu Chrome hinzufügen**.

   ![](assets/five.png)

1. Klicken Sie **Erweiterung hinzufügen**.

   ![](assets/six.png)

1. Zurück zu Marketo. Fügen Sie die Seiten-URL hinzu und klicken Sie auf **Vorschau**.

   ![](assets/seven.png)

1. Ein neues Fenster/eine neue Registerkarte wird geöffnet, in dem bzw. der Sie eine Vorschau des Erscheinungsbilds Ihrer Kampagne auf einem Desktop, Smartphone oder Tablet anzeigen können.

   ![](assets/campaign-preview.png)

## Vorschau einer Web-Kampagne auf der Web-Kampagnenseite {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Wenn Sie sich die Liste Ihrer Web-Kampagnen ansehen, wählen Sie einfach eine Kampagne aus und klicken Sie auf das Symbol **Vorschau**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Einfach!

## Vorschau einer Web-Kampagne auf Ihrer Website {#preview-a-web-campaign-on-your-website}

Erstellen Sie ein Sandbox-Segment und eine Kampagne.

1. Navigieren Sie zu **Segmente**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Klicken Sie auf **Neu erstellen**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Benennen Sie das Segment.

1. Ziehen Sie unter Verhalten die Option Einschließende Seiten auf die Arbeitsfläche. Fügen Sie den Wert &#42;sandbox=1) &#42;. Klicken Sie auf **Speichern und Kampagne definieren**.

   ![](assets/segment.png)

1. Ändern Sie auf der Seite Web-Kampagne festlegen das Zielsegment in das Sandbox-Segment, indem Sie es aus der Liste auswählen.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Schließen Sie die kreative Kampagne ab und klicken Sie auf **Starten**.

   ![](assets/click-launch.jpg)

1. Fügen Sie auf Ihrer Website den URL-Parameter &quot;?sandbox=1“ am Ende der URL hinzu. Beispiel: `www.marketo.com?sandbox=1`.

1. Zeigen Sie die Kampagne React auf Ihrer Website an.

>[!NOTE]
>
>Kampagnen reagieren nur einmal während einer Besuchersitzung. Um die Kampagne erneut zu sehen, löschen Sie Ihre Browser-Cookies.

>[!NOTE]
>
>Umleitungskampagnen können nicht in der Vorschau angezeigt werden. Die einzige Möglichkeit, sie zu testen, besteht in der Verwendung eines Sandbox-Segments (das bestimmte Seiten anspricht - &#42;sandbox=redirect&#42;)
