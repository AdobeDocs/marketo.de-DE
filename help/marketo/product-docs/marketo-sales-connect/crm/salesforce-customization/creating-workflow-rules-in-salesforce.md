---
unique-page-id: 14745823
description: Erstellen von Workflow-Regeln in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erstellen von Workflow-Regeln in Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# Erstellen von Workflow-Regeln in Salesforce {#creating-workflow-rules-in-salesforce}

Wenn Sie Marketo Sales Insight (MSI) und Marketo Sales Connect (MSC) parallel verwenden, wird die Funktion MSI Best Bets in Salesforce nicht aktualisiert. Alle anderen MSI-Funktionen funktionieren wie gewohnt (Anzeigen interessanter Momente im iFrame, Senden von E-Mails, Hinzufügen zu Kampagnen usw.). Dieser Artikel bietet eine Problemumgehung, damit Best Bets wieder funktionieren.

>[!NOTE]
>
>Dies betrifft nur Kunden, **sowohl** als auch MSE verwenden und die die Funktion Best Bets in MSI verwenden möchten. Wenn Sie keine Best Bets benötigen/verwenden, können Sie sie ignorieren.

## Erste Schritte {#getting-started}

Die Problemumgehung umfasst das Erstellen neuer Workflow-Regeln, um Werte aus neuen MSE-Feldern in die alten MSI-Felder zu kopieren. Sie müssen vier Workflow-Regeln für das Kontaktobjekt und dieselben vier Workflow-Regeln für das Lead-Objekt in Ihrer eigenen Salesforce-Instanz erstellen. Dazu müssen Sie möglicherweise über CRM-Administratorrechte verfügen (je nach Ihrer Rolle und Einrichtung im CRM).

Im Folgenden finden Sie die empfohlenen Namen der Workflow-Regeln und eine Beschreibung der einzelnen Regeln. Diese gelten für das Kontakt- und Lead-Objekt:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Feld für interessante Momentenbeschreibung aktualisieren</td> 
   <td><p>Kopieren von: Letzte Marketo Interaktion Beschreibung<br>Kopieren nach: Letzter interessanter Moment Beschreibung</p></td> 
  </tr> 
  <tr> 
   <td>Feld für interessanten Moment aktualisieren</td> 
   <td><p>Kopieren von: Letzter Marketo-Interaktionstyp<br>Kopieren nach: Typ des letzten interessanten Moments</p></td> 
  </tr> 
  <tr> 
   <td>Source-Feld „Interessante Momente aktualisieren“</td> 
   <td><p>Kopieren von: Letzte Marketo Interaktion Source<br>Kopieren nach: Letzter interessanter Moment Source</p></td> 
  </tr> 
  <tr> 
   <td>Feld für interessante Momente aktualisieren</td> 
   <td><p>Kopieren von: Letztes Marketo-Interaktionsdatum<br>Kopieren nach: Letztes interessantes Momentendat</p></td> 
  </tr> 
 </tbody> 
</table>

## Anleitung {#instructions}

1. Nachdem Sie auf **Setup** geklickt haben, suchen Sie nach **Workflow** und wählen Sie **Workflow-Regeln**.

   ![](assets/one-1.png)

1. Wählen Sie **Neue Regel** aus.

   ![](assets/two-1.png)

1. Klicken Sie auf die Dropdown-Liste Objekt und wählen Sie **Lead** und klicken Sie dann auf **Weiter**.

   ![](assets/three-1.png)

1. Geben Sie als Regelnamen „Feld für interessanten Moment aktualisieren“ ein. Wählen Sie die Optionsschaltfläche **erstellt und jedes Mal, wenn sie bearbeitet wird** aus. Wählen Sie in der Dropdown-Liste Regelkriterien die Option **Formel wird als „true“ ausgewertet**. Suchen Sie nach der Funktion ISCHANGED und wählen Sie sie aus. Markieren Sie dann den Wert des Standardfelds und klicken Sie auf **Feld einfügen**.

   ![](assets/four-1.png)

1. Wählen Sie im Pop-up „Feld einfügen“ die Option **Letzte Marketo-Interaktionsbeschreibung** und klicken Sie auf **Einfügen**.

   ![](assets/five-1.png)

1. Klicken Sie **Speichern und Weiter**.

   ![](assets/6.png)

1. Wählen Sie in der Dropdown-Liste Workflow-Aktion hinzufügen die Option **Neues Feld aktualisieren**.

   ![](assets/seven.png)

1. Geben Sie in das Feld „Name“ „Feld für Beschreibung des interessanten Moments aktualisieren“ ein (eindeutiger Name wird automatisch generiert). Wählen Sie in der Dropdown-Liste Zu aktualisierendes Feld **Beschreibung des letzten interessanten Moments**. Wählen Sie das Optionsfeld **Formel zum Festlegen eines neuen Werts verwenden** und klicken Sie dann auf **Formeleditor anzeigen**.

   ![](assets/eight.png)

1. Klicken Sie auf **Schaltfläche** Feld einfügen“.

   ![](assets/9a.png)

1. Wählen Sie **Letzte Marketo-Interaktionsbeschreibung** aus und klicken Sie auf **Einfügen**. Klicken Sie auf der nächsten Seite auf **Speichern**.

   ![](assets/nine.png)

1. Klicken Sie auf **Fertig**.

   ![](assets/twelve.png)

1. Klicken Sie **Aktivieren**, um die Workflow-Regel zu aktivieren.

   ![](assets/thirteen.png)

   Nach dem letzten Schritt können Sie die Workflow-Regel für die anderen Felder klonen, die im Abschnitt Erste Schritte aufgeführt sind: Beschreibung, Typ, Source, Datum. Nachdem Sie die vier Workflow-Regeln im Kontaktobjekt abgeschlossen haben, wiederholen Sie dies für das Lead-Objekt.
