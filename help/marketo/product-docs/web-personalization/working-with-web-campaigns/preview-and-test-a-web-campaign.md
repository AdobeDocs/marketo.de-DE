---
unique-page-id: 10092925
description: Vorschau und Testen einer Webkampagne - Marketo-Dokumente - Produktdokumentation
title: Vorschau erstellen und eine Webkampagne testen
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Vorschau erstellen und eine Webkampagne testen {#preview-and-test-a-web-campaign}

Dieser Artikel zeigt Ihnen verschiedene Möglichkeiten, eine Webkampagne in der Vorschau anzuzeigen, und wie Sie sie auch mithilfe eines Sandbox-Segments live auf Ihrer Website testen können.

>[!NOTE]
>
>Die Vorschau zeigt nur, wie die Kampagne auf der ausgewählten Site aussehen wird. Links und Widgets sind nicht funktionsfähig, um fehlerhafte Klicks/Ansichten in der Analyse zu vermeiden.

## Vorschau einer Webkampagne auf der Erstellungsseite {#preview-a-web-campaign-on-the-creation-page}

1. Gehen Sie zu **Web-Kampagnen**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Klicken Sie auf **Neue Web-Kampagne erstellen** oder auf das Symbol, um eine bestehende Kampagne zu bearbeiten.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Fügen Sie in der Vorschau auf der Site die Seiten-URL hinzu und klicken Sie auf **Vorschau**. Ein neues Fenster bzw. eine neue Registerkarte mit der Kampagnenvorschau wird geöffnet.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Klicken Sie auf **Share** , um eine E-Mail mit einer festen URL der Kampagnenvorschau zu öffnen.

   >[!NOTE]
   >
   >Sie haben auch die Möglichkeit, ein Browser-Plug-in zu installieren (entweder [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) oder [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)), um eine optimale Kampagnenvorschau zu erhalten. Siehe den Abschnitt unten.

## Vorschau einer Webkampagne auf der Erstellungsseite mithilfe des Browser-Plug-ins {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Führen Sie die Schritte 1 und 2 aus dem obigen Abschnitt aus.

1. Klicken Sie auf den Link zum Browser-Plug-in (in diesem Fall verwenden wir Chrome).

   ![](assets/4-1.png)

1. Ein neues Fenster/eine neue Registerkarte wird geöffnet. Klicken Sie auf **Zu Chrome** hinzufügen.

   ![](assets/five.png)

1. Klicken Sie auf **Erweiterung hinzufügen**.

   ![](assets/six.png)

1. Gehen Sie zurück zu Marketo. Fügen Sie die Seiten-URL hinzu und klicken Sie auf **Vorschau**.

   ![](assets/seven.png)

1. Daraufhin wird ein neues Fenster/eine neue Registerkarte geöffnet, in dem Sie sich ansehen können, wie Ihre Kampagne auf einem Desktop-PC, Smartphone oder Tablet aussieht.

   ![](assets/campaign-preview.png)

## Vorschau einer Webkampagne auf der Seite &quot;Webkampagnen&quot; {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Wenn Sie sich die Liste Ihrer Webkampagnen ansehen, wählen Sie einfach eine Kampagne aus und klicken Sie auf das Symbol **Vorschau**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Einfach!

## Vorschau einer Webkampagne auf Ihrer Website {#preview-a-web-campaign-on-your-website}

Erstellen Sie ein Sandbox-Segment und eine Kampagne.

1. Navigieren Sie zu **Segmente**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Klicken Sie auf **Neu erstellen**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Benennen Sie das Segment.

1. Ziehen Sie unter &quot;Verhalten&quot;Seiten einschließen auf die Arbeitsfläche. Fügen Sie den Wert *sandbox=1* hinzu. Klicken Sie auf **Kampagne speichern und definieren**.

   ![](assets/segment.png)

1. Ändern Sie auf der Seite Webkampagne festlegen das Zielsegment in das Sandbox-Segment, indem Sie es aus der Liste auswählen.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Vervollständigen Sie die Kampagne und klicken Sie auf **Launch**.

   ![](assets/click-launch.jpg)

1. Fügen Sie auf Ihrer Website den URL-Parameter &quot;?sandbox=1&quot;am Ende der URL hinzu. Beispiel: `www.marketo.com?sandbox=1`.

1. Sehen Sie sich die Kampagnenreaktion auf Ihrer Website an.

>[!NOTE]
>
>Kampagnen reagieren nur einmal während einer Besuchersitzung. Um die Kampagne erneut anzuzeigen, löschen Sie Ihre Browser-Cookies.

>[!NOTE]
>
>Umleitungskampagnen können nicht in der Vorschau angezeigt werden. Die einzige Möglichkeit, sie zu testen, ist die Verwendung eines Sandbox-Segments (das auf bestimmte Seiten ausgerichtet ist - *sandbox=redirect*).
