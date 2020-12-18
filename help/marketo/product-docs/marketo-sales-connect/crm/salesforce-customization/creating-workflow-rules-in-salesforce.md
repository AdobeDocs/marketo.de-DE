---
unique-page-id: 14745823
description: Erstellen von Workflow-Regeln in Salesforce - Marketing Docs - Produktdokumentation
title: Erstellen von Workflow-Regeln in Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Erstellen von Workflow-Regeln in Salesforce {#creating-workflow-rules-in-salesforce}

Bei gleichzeitiger Verwendung von Marketo Sales Insight (MSI) und Marketo Sales Connect (MSC) wird die Funktion MSI Best Bets in Salesforce nicht aktualisiert. Alle anderen MSI-Funktionen funktionieren wie gewohnt (Anzeige interessanter Momente im iFrame, Senden von E-Mails, Hinzufügen zu Kampagnen usw.). In diesem Artikel wird eine Problemumgehung Angebot, damit die Best-Bets-Version wieder funktioniert.

>[!NOTE]
>
>Dies betrifft nur Kunden, die **sowohl** MSI als auch MSE verwenden und die die Funktion &quot;Beste Einsätze&quot;in MSI verwenden möchten. Wenn Sie keine Best Bets benötigen/verwenden, können Sie ignorieren.

## Erste Schritte {#getting-started}

Die Problemumgehung umfasst das Erstellen neuer Workflow-Regeln, um Werte aus neuen MSE-Feldern in die alten MSI-Felder zu kopieren. Sie müssen vier Workflow-Regeln für das Kontaktobjekt und die gleichen vier Workflow-Regeln für das Lead-Objekt in Ihrer eigenen Salesforce-Instanz erstellen. Dies erfordert möglicherweise, dass Sie über CRM-Administratorrechte verfügen (je nach Ihrer Rolle und Einrichtung in CRM).

Nachfolgend finden Sie die empfohlenen Namen der Workflow-Regeln und Beschreibungen der einzelnen Regeln. Diese gelten für das Kontaktobjekt und das Interessentenobjekt:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Interaktives Moment-Desc-Feld aktualisieren</td> 
   <td><p>Kopieren von: Letzter Marker für Interaktion Desc<br>Kopieren nach: Letzter interessanter Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td>Feld "Interessanter Moment-Typ aktualisieren"</td> 
   <td><p>Kopieren von: Letzter Markierungstyp für Interaktion<br>Kopieren nach: Letzter interessanter Moment-Typ</p></td> 
  </tr> 
  <tr> 
   <td>Feld "Interessantes Moment aktualisieren"</td> 
   <td><p>Kopieren von: Letzter Markt für Interaktionsquelle<br>Kopieren nach: Letzter interessanter Moment Quelle</p></td> 
  </tr> 
  <tr> 
   <td>Feld "Interessantes Datum aktualisieren"</td> 
   <td><p>Kopieren von: Letztes Markierungsbindungsdatum<br>Kopieren nach: Datum des letzten interessanten Moments</p></td> 
  </tr> 
 </tbody> 
</table>

## Anweisungen {#instructions}

1. Suchen Sie nach **Setup**, suchen Sie nach **Workflow** und wählen Sie **Workflow-Regeln**.

   ![](assets/one-1.png)

1. Wählen Sie **Neue Regel**.

   ![](assets/two-1.png)

1. Klicken Sie auf die Dropdown-Liste &quot;Objekt&quot;und wählen Sie **Lead** und klicken Sie dann auf **Weiter**.

   ![](assets/three-1.png)

1. Geben Sie als Regelnamen &quot;Update Interest Moment Desc Field&quot;ein. Wählen Sie das Optionsfeld **erstellt und jedes Mal, wenn es bearbeitet wird**. Wählen Sie in der Dropdownliste Regelkriterien **Formel wird als true** ausgewertet. Suchen Sie die Funktion ISCHANGED und wählen Sie sie aus. Markieren Sie dann den Standardwert für das Feld und klicken Sie auf **Feld** einfügen.

   ![](assets/four-1.png)

1. Wählen Sie im Popup &quot;Feld einfügen&quot;die Option **Letzter Marker für Interaktion Desc** und klicken Sie auf **Einfügen**.

   ![](assets/five-1.png)

1. Klicken Sie auf **Speichern &amp; Weiter**.

   ![](assets/6.png)

1. Wählen Sie in der Dropdown-Liste Hinzufügen-Aktion die Option **Neues Feldupdate**.

   ![](assets/seven.png)

1. Geben Sie im Feld Name die Bezeichnung &quot;Update Interested Moment Desc Field&quot; ein (Unique Name wird automatisch generiert). Wählen Sie in der Dropdownliste Zu aktualisierendes Feld **Letzter interessanter Moment Desc**. Wählen Sie das Optionsfeld **Verwenden Sie eine Formel, um einen neuen Wert** festzulegen, und klicken Sie dann auf **Formel-Editor anzeigen**.

   ![](assets/eight.png)

1. Klicken Sie auf die Schaltfläche **Feld** einfügen.

   ![](assets/9a.png)

1. Wählen Sie **Letzter Marker für Interaktion Desc** und klicken Sie auf **Einfügen**. Klicken Sie auf der nächsten Seite auf **Speichern**.

   ![](assets/nine.png)

1. Klicken Sie auf **Fertig**.

   ![](assets/twelve.png)

1. Klicken Sie auf **Aktivieren**, um die Workflow-Regel zu aktivieren.

   ![](assets/thirteen.png)

   Nach dem letzten Schritt können Sie die Workflow-Regel für die anderen Felder klonen, die im Abschnitt &quot;Erste Schritte&quot;aufgeführt sind: Desc, Typ, Quelle, Datum. Nachdem Sie die vier Workflow-Regeln im Kontaktobjekt abgeschlossen haben, wiederholen Sie dies für das Lead-Objekt.

