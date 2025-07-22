---
unique-page-id: 14745823
description: Erstellen von Workflow-Regeln in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erstellen von Workflow-Regeln in Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# Erstellen von Workflow-Regeln in Salesforce {#creating-workflow-rules-in-salesforce}

Wenn Sie Marketo Sales Insight (MSI) und Marketo Sales Connect (MSC) parallel verwenden, wird die Funktion MSI Best Bets in [!DNL Salesforce] nicht aktualisiert. Alle anderen MSI-Funktionen funktionieren wie gewohnt (Anzeigen interessanter Momente im iFrame, Senden von E-Mails, Hinzufügen zu Kampagnen usw.). Dieser Artikel bietet eine Problemumgehung, damit Best Bets wieder funktionieren.

>[!NOTE]
>
>Dies betrifft nur Kunden, **sowohl** als auch MSE verwenden und die die Funktion Best Bets in MSI verwenden möchten. Wenn Sie keine Best Bets benötigen/verwenden, können Sie sie ignorieren.

## Erste Schritte {#getting-started}

Die Problemumgehung umfasst das Erstellen neuer Workflow-Regeln, um Werte aus neuen MSE-Feldern in die alten MSI-Felder zu kopieren. Sie müssen vier Workflow-Regeln für das Kontaktobjekt und dieselben vier Workflow-Regeln für das Lead-Objekt in Ihrer eigenen [!DNL Salesforce] erstellen. Dazu müssen Sie möglicherweise über CRM-Administratorrechte verfügen (je nach Ihrer Rolle und Einrichtung im CRM).

Im Folgenden finden Sie die empfohlenen Namen der Workflow-Regeln und eine Beschreibung der einzelnen Regeln. Diese gelten für die Objekte [!UICONTROL Kontakt] und [!UICONTROL Lead]:

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

1. Nachdem Sie auf **[!UICONTROL Setup]** geklickt haben, suchen Sie nach **Workflow** und wählen Sie **[!UICONTROL Workflow-Regeln]**.

   ![](assets/one-1.png)

1. Wählen Sie **[!UICONTROL Neue Regel]** aus.

   ![](assets/two-1.png)

1. Klicken Sie auf [!UICONTROL Objekt] Dropdown-Liste und wählen Sie **[!UICONTROL Lead]** und klicken Sie dann auf **[!UICONTROL Weiter]**.

   ![](assets/three-1.png)

1. Geben Sie als [!UICONTROL Regelname“ „Feld für interessanten Moment aktualisieren] ein. Wählen Sie die Optionsschaltfläche **[!UICONTROL erstellt und jedes Mal, wenn sie bearbeitet wird]** aus. Wählen Sie in [!UICONTROL  Dropdown-Liste ]Regelkriterien“ **[!UICONTROL Formel wird als „true“ ausgewertet]**. Suchen Sie nach der Funktion ISCHANGED und wählen Sie sie aus. Markieren Sie dann den Wert des Standardfelds und klicken Sie auf **[!UICONTROL Feld einfügen]**.

   ![](assets/four-1.png)

1. Wählen Sie im Pop-up [!UICONTROL Feld einfügen] die Option **[!UICONTROL Letzter Marketo-]**) und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/five-1.png)

1. Klicken Sie **[!UICONTROL Speichern und Weiter]**.

   ![](assets/6.png)

1. Wählen Sie in [!UICONTROL  Dropdown-Liste ]Workflow-Aktion hinzufügen **[!UICONTROL die Option „Neues Feld aktualisieren]**.

   ![](assets/seven.png)

1. Geben Sie [!UICONTROL  Feld „Name] „Feld für interessanten Moment aktualisieren“ ein ([!UICONTROL Eindeutiger Name] wird automatisch generiert). Wählen Sie in [!UICONTROL  Dropdown-Liste ]Zu aktualisierendes Feld“ die Option **[!UICONTROL Beschreibung des letzten interessanten Moments]**. Wählen Sie das Optionsfeld **[!UICONTROL Formel zum Festlegen eines neuen Werts verwenden]** und klicken Sie dann auf **[!UICONTROL Formeleditor anzeigen]**.

   ![](assets/eight.png)

1. Klicken Sie auf **[!UICONTROL Schaltfläche]** Feld einfügen“.

   ![](assets/9a.png)

1. Wählen Sie **[!UICONTROL Letzte Marketo-Interaktionsbeschreibung]** aus und klicken Sie auf **[!UICONTROL Einfügen]**. Klicken Sie auf der nächsten Seite auf **[!UICONTROL Speichern]**.

   ![](assets/nine.png)

1. Klicken Sie auf **[!UICONTROL Fertig]**.

   ![](assets/twelve.png)

1. Klicken Sie **[!UICONTROL Aktivieren]**, um die Workflow-Regel zu aktivieren.

   ![](assets/thirteen.png)

   Nach dem letzten Schritt können Sie die Workflow-Regel für die anderen Felder klonen, die im Abschnitt [!UICONTROL Erste Schritte] aufgeführt sind: Beschreibung, Typ, Source, Datum. Nachdem Sie die vier Workflow-Regeln im Objekt [!UICONTROL Kontakt] abgeschlossen haben, wiederholen Sie dies für das Objekt [!UICONTROL Lead].
