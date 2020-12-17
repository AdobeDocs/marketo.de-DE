---
unique-page-id: 4719304
description: Implizierte Salesforce-Aktionen - Marketing Docs - Produktdokumentation
title: Implizierte Salesforce-Aktionen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Implizierte Salesforce-Aktionen {#implied-salesforce-actions}

Wenn ein Salesforce-spezifischer Flussschritt ausgeführt wird, werden manchmal zusätzliche Schritte automatisch ausgeführt. Hier sind die Regeln, Sie wissen also:

Diese Regeln gelten für *wenn sich die Person derzeit nicht unter [Salesforce.com](http://Salesforce.com)* als Kontakt oder Interessent befindet.

<table> 
 <thead> 
  <tr> 
   <th>Schritt zum Markieren</th> 
   <th>Automatische Aktion</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>hinzufügen an die SFDC-Kampagne</td> 
   <td>Person mit dem SFDC synchronisieren</td> 
  </tr> 
  <tr> 
   <td>Status in der SFDC-Kampagne ändern</td> 
   <td>Person mit SFDC<br>Hinzufügen mit SFDC-Kampagne synchronisieren</td> 
  </tr> 
  <tr> 
   <td>Inhaber ändern</td> 
   <td><p>Person mit dem SFDC synchronisieren</p></td> 
  </tr> 
  <tr> 
   <td>Person konvertieren</td> 
   <td><p>Person mit dem SFDC synchronisieren</p></td> 
  </tr> 
  <tr> 
   <td>Aufgabe erstellen</td> 
   <td>Person mit dem SFDC synchronisieren</td> 
  </tr> 
 </tbody> 
</table>

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des Filters **SFDC-Typ** herausfiltern, wobei der Operator auf &quot;ist nicht leer&quot;gesetzt ist. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Beachten Sie, dass diese automatischen Aktionen nur stattfinden, wenn der Interessent derzeit nicht unter [Salesforce.com](http://Salesforce.com)

Die Salesforce-Synchronisierung ist cool, nicht wahr?
