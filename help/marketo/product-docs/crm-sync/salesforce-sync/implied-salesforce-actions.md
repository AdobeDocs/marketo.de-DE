---
unique-page-id: 4719304
description: Implizierte Salesforce-Aktionen - Marketo Docs - Produktdokumentation
title: Implizierte Salesforce-Aktionen
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Implizierte Salesforce-Aktionen {#implied-salesforce-actions}

Wenn ein Salesforce-spezifischer Flussschritt ausgeführt wird, werden manchmal zusätzliche Schritte automatisch ausgeführt. Hier sind die Regeln, Sie wissen also:

Diese Regeln gelten für _wenn sich die Person derzeit nicht unter [Salesforce.com](https://Salesforce.com)_ als Kontakt oder Interessent befindet.

<table> 
 <thead> 
  <tr> 
   <th>Marketo-Flussschritt</th> 
   <th>Automatische Aktion</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Zu SFDC-Kampagne hinzufügen</td> 
   <td>Person mit SFDC synchronisieren</td> 
  </tr> 
  <tr> 
   <td>Status in SFDC-Kampagne ändern</td> 
   <td>Person mit SFDC<br>Hinzufügen mit SFDC-Kampagne synchronisieren</td> 
  </tr> 
  <tr> 
   <td>Eigentümer ändern</td> 
   <td><p>Person mit SFDC synchronisieren</p></td> 
  </tr> 
  <tr> 
   <td>Person konvertieren</td> 
   <td><p>Person mit SFDC synchronisieren</p></td> 
  </tr> 
  <tr> 
   <td>Aufgabe erstellen</td> 
   <td>Person mit SFDC synchronisieren</td> 
  </tr> 
 </tbody> 
</table>

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des Filters **SFDC-Typ** herausfiltern, wobei der Operator auf &quot;ist nicht leer&quot;gesetzt ist. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Beachten Sie, dass diese automatischen Aktionen nur stattfinden, wenn der Interessent derzeit nicht unter [Salesforce.com](https://salesforce.com)
