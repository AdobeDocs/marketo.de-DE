---
unique-page-id: 4719400
description: Erstellen einer neuen Web-Kampagne in Zone - Marketo Docs - Produktdokumentation
title: Erstellen einer neuen Web-Kampagne in Zone
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 1%

---

# Erstellen einer neuen Web-Kampagne in Zone {#create-a-new-in-zone-web-campaign}

Eine Webkampagne ist eine angepasste Reaktion, die mit einem bestimmten Segment verknüpft ist. Dabei kann es sich um ein [Dialogfeld](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) auf Ihrer Website, einen In-Zone-Austausch, eine [Widget-Funktion](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) oder einen E-Mail-Warnhinweis handeln. Eine Web-Kampagne in Zone ersetzt ein Element Ihrer Website, das auf der Zone-ID basiert, durch Inhalte oder grafische Banner.

## Erstellen einer Web-Kampagne für In-Zone {#create-an-in-zone-web-campaign}

1. Wechseln Sie zu **Web-Kampagnen**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Wählen Sie **Neue Webkampagne erstellen.**

   ![](assets/create-new-web-campaign-hand.png)

1. Wählen Sie den Kampagnentyp **In Zone** aus. Passen Sie die Bereichs-ID &quot;**an und fügen Sie sie hinzu.** Setzen Sie die Kampagne auf &quot;**Sticky**&quot; und fügen Sie Ihr kreatives Element im Editor hinzu. Fügen Sie die URL der Seite hinzu, die Sie in der Vorschau anzeigen möchten, und klicken Sie auf **Vorschau** , um zu sehen, wie die Kampagne auf Ihrer Site reagieren wird.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Was ist eine Zone-ID?**
   >
   >Eine Zone-ID ist der Bereich, in dem sich Ihre Web-Kampagne &quot;In Zone&quot;auf der Site befinden soll. Um eine &quot;Zonen-ID&quot;zu finden, wählen Sie einfach auf Ihrer Website den Bereich aus, den Sie durch eine Web-Kampagne ersetzen möchten, und klicken Sie mit der rechten Maustaste darauf. In Chrome ist die Option &quot;Inspect-Element&quot;und kann in anderen Browsern variieren.
   >
   >Dann suchen Sie die &quot;id&quot;, die mit diesem Bereich der Website verknüpft ist, der hervorgehoben wird, da Sie dieses Element überprüfen. Wenn beispielsweise nach einem Rechtsklick in Chrome der markierte Text `<div id="featured-slider">` lautet, dann sollte der &quot;Regler für spezielle Funktionen&quot;im Abschnitt &quot;Zone ID&quot;eingegeben werden. In der Regel wird &quot;div id&quot;verwendet, es kann jedoch auch eine beliebige ID verwendet werden, z. B. h1 id, p id usw.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Name</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> Bereichs-ID </strong></td> 
   <td colspan="1" rowspan="1"><p>Geben Sie den Namen der ID im HTML-Code Ihres Website-Elements ein, das durch die Kampagne ersetzt wird.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Anhaftend </strong></p></td> 
   <td colspan="1" rowspan="1">Das Kontrollkästchen "Sticky"ist standardmäßig für die In-Zone-Kampagne aktiviert und behält die In-Zone-Kampagne während der gesamten Besuchersitzung auf der Website an ihrer Zone-ID-Position bei. Es wird empfohlen, immer eine In-Zone auf "Sticky"festzulegen.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Überblendung</strong> </p></td> 
   <td colspan="1" rowspan="1">Wenn Sie das Kontrollkästchen "Effekt verwenden"und "Ausblenden"aktivieren, wird der Bereich der Bereich-ID auf der Website ausgeblendet. Wenn es sich bei der In-Zone um ein grafisches Banner handelt, wird die Seite zuerst geladen und dann die Kampagne mit verblassender Wirkung aktiviert.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Gleiten</strong></td> 
   <td colspan="1">Wenn Sie das Kontrollkästchen "Effekt verwenden"und die Option "Verschieben"aktivieren, wird der Bereich der Bereich-ID auf der Website eingeblendet. Wenn es sich bei der In-Zone um ein grafisches Banner handelt, wird die Seite zuerst geladen und dann wird die Kampagne mit einem beweglichen Effekt von links nach rechts aktiviert.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> RTF-Editor  </strong></td> 
   <td colspan="1">Der Rich-Text-Editor ermöglicht die Textformatierung, Verknüpfung und Einfügen von Bildern. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Mehr dazu hier</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Vorschau auf Website   </strong></td> 
   <td colspan="1">Anzeigen einer Vorschau von Kampagnen vor dem Start <br> 
    <ul> 
     <li> URL - Geben Sie eine Beispiel-URL ein, unter der die Kampagne laufen würde, um ein Vorschaubeispiel dafür zu erhalten, wie die Kampagne live aussehen würde.</li> 
     <li>Gerät - Sehen Sie sich an, wie Ihre Kampagne auf dem Gerät dargestellt wird: Desktop, Mobiles Hochformat, Mobilgerät - Querformat, Tablet - Hochformat, Hochformat.</li> 
     <li> Vorschau - Klicken Sie auf <strong>Vorschau</strong> , um ein neues Fenster der Beispiel-URL zu öffnen und zu sehen, wie die Kampagne reagiert.</li> 
     <li> Freigabe - Verwenden Sie die Schaltfläche Freigeben , um eine E-Mail an einen Kollegen mit einem Link zu senden, um die Proxy-Kampagne anzuzeigen.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Beschleunigen und vereinfachen Sie den Kampagnenerstellungsprozess, indem Sie unsere [integrierten Vorlagen](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) oder Ihre vorhandene Kampagne](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) als Vorlage zur Wiederverwendung speichern.[

>[!NOTE]
>
>**Möchten Sie Ihre Web-Kampagnen A/B testen?** Mindestens eine Webkampagne kann [A/B-Test auf optimale Ergebnisse sein](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Mit der Funktion Automatisierte Abstimmung erkennt die Plattform automatisch die leistungsschwächeren Kampagnen, setzt die Kampagne mit der höchsten Konversionsrate fort und setzt die anderen Kampagnen aus.

## Eine Webkampagne bearbeiten {#edit-a-web-campaign}

Klicken Sie auf der Seite **Web-Kampagnen** in der Kampagne auf **Bearbeiten** .

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Um die gewünschte Kampagne leichter zu finden, verwenden Sie die [Filterfunktion](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Vorschau einer Webkampagne {#preview-a-web-campaign}

1. Klicken Sie auf der Web-Kampagnenseite in der Webkampagne, die Sie anzeigen möchten, auf **Vorschau** .

   ![](assets/in-zone-web-campaign-preview.png)

## Eine Webkampagne klonen {#clone-a-web-campaign}

Siehe [Eine Webkampagne klonen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Eine Webkampagne löschen {#delete-a-web-campaign}

1. Klicken Sie auf der Seite Web-Kampagnen auf **Löschen** in der Kampagne, die Sie löschen möchten.

   ![](assets/in-zone-web-campaign-delete.png)

1. Eine Bestätigungsmeldung wird angezeigt, um zu bestätigen, ob Sie die Kampagne löschen möchten.

>[!MORELIKETHIS]
>
>* [Erstellen einer neuen Widget-Web-Kampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Erstellen einer neuen Webkampagne für ein Dialogfeld](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
