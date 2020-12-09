---
unique-page-id: 4719400
description: Neue Web-Kampagne für die Zone - Marketing Docs - Produktdokumentation erstellen
title: Eine neue Web-Kampagne in einer Zone erstellen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---


# Eine neue Web-Kampagne in einer Zone erstellen {#create-a-new-in-zone-web-campaign}

Eine Web-Kampagne ist eine benutzerspezifische Reaktion, die mit einem bestimmten Segment verknüpft ist. Dabei kann es sich um ein [Dialogfeld](create-a-new-dialog-web-campaign.md) auf Ihrer Website, einen In-Zone-Ersatz, eine [Widget-Funktion](create-a-new-widget-web-campaign.md) oder eine E-Mail-Warnung handeln. Eine In-Zone-Web-Kampagne ersetzt ein auf der Zone-ID basierendes Element Ihrer Website durch Inhalte oder grafische Banner.

## Eine In-Zone-Web-Kampagne erstellen {#create-an-in-zone-web-campaign}

1. Gehen Sie zu **Web-Kampagnen**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Wählen Sie Neue Web-Kampagne **erstellen.**

   ![](assets/create-new-web-campaign-hand.png)

1. Wählen Sie die Kampagne **für die In-Zone** aus. Passen Sie die **Zonen-ID an und fügen Sie sie hinzu.** Legen Sie die Kampagne auf **Sticky** fest und fügen Sie Ihre kreativen Elemente im Editor hinzu. hinzufügen Sie die URL der Seite zur Vorschau und klicken Sie auf **Vorschau** , um zu sehen, wie die Kampagne auf Ihrer Site reagiert.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >
   >**Was ist eine Zone-ID?**
   >
   >
   >Eine Zone-ID ist der Ort, an dem sich Ihre &quot;In-Zone&quot;-Kampagne auf der Site befinden soll. Um eine &quot;Zone-ID&quot; zu finden, gehen Sie einfach zu Ihrer Website wählen Sie den Bereich, den Sie durch eine Web-Kampagne ersetzen möchten und klicken Sie mit der rechten Maustaste. In Chrome ist die Option &quot;Inspect Element&quot;, in anderen Browsern kann sie variieren.
   >
   >
   >Dann suchen Sie die mit diesem Abschnitt der Website verknüpfte ID, die hervorgehoben wird, da Sie dieses Element überprüfen. Wenn Sie z. B. nach einem Rechtsklick in Chrome den markierten Text anklicken, lautet `<div id="featured-slider">` dann &quot;Regler mit speziellen Funktionen&quot;was Sie im Abschnitt &quot;Zonen-ID&quot;eingeben sollten. Normalerweise wird &quot;div id&quot;verwendet, es können aber auch beliebige IDs wie h1 id, p id usw. verwendet werden.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Name</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> Zone-ID </strong></td> 
   <td colspan="1" rowspan="1"><p>Geben Sie den Namen der ID ein, die im HTML-Code des Elements Ihrer Website enthalten ist, das die Kampagne ersetzt.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Sticky </strong></p></td> 
   <td colspan="1" rowspan="1">Das Kontrollkästchen "Stickiness"ist standardmäßig für die In-Zone-Kampagne aktiviert und behält die In-Zone-Kampagne während der gesamten Sitzung des Besuchers auf der Website in ihrer Zone-ID. Es wird empfohlen, immer eine In-Zone auf Sticky festzulegen.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Überblendung</strong> </p></td> 
   <td colspan="1" rowspan="1">Wenn Sie das Kontrollkästchen "Effekt verwenden"und "Überblenden"aktivieren, wird der Bereich "Zonen-ID"auf der Website ausgeblendet. Wenn es sich bei der In-Zone um ein grafisches Banner handelt, wird die Seite zuerst geladen und dann wird die Kampagne mit einem Überblendeffekt aktiviert.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Schieben</strong></td> 
   <td colspan="1">Wenn Sie das Kontrollkästchen "Effekt verwenden"und die Option "Sliding"aktivieren, wird der Bereich "Zone-ID"auf der Website verschoben. Wenn es sich bei der In-Zone um ein grafisches Banner handelt, wird die Kampagne zuerst geladen und dann mit einem gleitenden Effekt von links nach rechts aktiviert.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Rich-Text-Editor  </strong></td> 
   <td colspan="1">Der Rich-Text-Editor ermöglicht die Textformatierung, Verknüpfung und Einfügen von Bildern. <a href="using-the-web-personalization-rich-text-editor.md">Mehr dazu hier</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Vorschau vor Ort   </strong></td> 
   <td colspan="1">Kampagnen zur Vorschau vor dem Start. <br> 
    <ul> 
     <li> URL - Geben Sie eine Beispiel-URL ein, unter der die Kampagne ausgeführt wird, um ein Beispiel für die Vorschau der Live-Darstellung der Kampagne anzuzeigen.</li> 
     <li>Gerät - Vorschau, wie Ihre Kampagne auf dem Gerät angezeigt wird: Desktop, mobiles Hochformat, Mobile Querformat, Tablet Hochformat, Hochformat.</li> 
     <li> Vorschau - Klicken Sie auf <strong>Vorschau</strong> , um ein neues Fenster der Beispiel-URL zu öffnen, um zu sehen, wie die Kampagne reagiert.</li> 
     <li> Freigeben: Verwenden Sie die Schaltfläche Freigeben, um eine E-Mail an einen Kollegen mit einem Link zu senden, um die Proxy-Kampagne anzuzeigen.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Beschleunigen und vereinfachen Sie die Erstellung Ihrer Kampagne, indem Sie unsere [integrierten Vorlagen](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) verwenden oder Ihre vorhandene Kampagne [als Vorlage zur Wiederverwendung](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) speichern.

>[!NOTE]
>
>**Möchten Sie Ihre Web-Kampagnen A/B testen?** Eine oder mehrere Web-Kampagnen können [A/B auf optimale Ergebnisse](ab-test-your-web-campaign.md)getestet werden. Mit der Auto-Tune-Funktion erkennt die Plattform automatisch die leistungsfähigeren Kampagnen, setzt die Kampagnen mit der höchsten Umrechnung fort und hält die anderen an.

## Eine Web-Kampagne bearbeiten {#edit-a-web-campaign}

Klicken Sie auf der Seite **Web-Kampagnen** auf der Kampagne auf **Bearbeiten** .

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Um die gewünschte Kampagne leichter zu finden, verwenden Sie die [Filterfunktion](filter-web-campaigns.md).

## Vorschau einer Web-Kampagne {#preview-a-web-campaign}

1. Klicken Sie auf der Seite &quot;Web-Kampagnen&quot;auf **Vorschau **auf der Web-Kampagne, die Sie Ansicht wünschen.

   ![](assets/in-zone-web-campaign-preview.png)

## Klonen einer Web-Kampagne {#clone-a-web-campaign}

Siehe [Klonen einer Web-Kampagne](clone-a-web-campaign.md).

## Eine Web-Kampagne löschen {#delete-a-web-campaign}

1. Klicken Sie auf der Seite &quot;Web-Kampagnen&quot;auf **Löschen **auf der Kampagne, die Sie löschen möchten.

   ![](assets/in-zone-web-campaign-delete.png)

1. Es wird eine Bestätigungsmeldung angezeigt, die bestätigt, ob Sie die Kampagne löschen möchten.

>[!MORELIKETHIS]
>
>* [Neue Widget-Web-Kampagne erstellen](create-a-new-widget-web-campaign.md)
>* [Eine neue Dialogfeld-Web-Kampagne erstellen](create-a-new-dialog-web-campaign.md)

