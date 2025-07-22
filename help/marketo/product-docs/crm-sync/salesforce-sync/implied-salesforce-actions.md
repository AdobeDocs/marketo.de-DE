---
unique-page-id: 4719304
description: Implizite Salesforce-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Implizite Salesforce-Aktionen
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 21%

---

# Implizite Salesforce-Aktionen {#implied-salesforce-actions}

Wenn ein [!DNL Salesforce] Flussschritt ausgeführt wird, werden manchmal zusätzliche Schritte automatisch ausgeführt. Hier sind die Regeln, also wissen Sie:

Diese Regeln gelten, wenn sich die Person derzeit nicht in [Salesforce.com](https://Salesforce.com){target="_blank"} als Kontakt oder Lead befindet.

<table> 
 <thead> 
  <tr> 
   <th>Marketo-Flussschritt</th> 
   <th>automatische Handlung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Zu SFDC-Kampagne hinzufügen</td> 
   <td>Person mit SFDC synchronisieren</td> 
  </tr> 
  <tr> 
   <td>Status in SFDC-Kampagne ändern</td> 
   <td>Person mit SFDC synchronisieren<br> Zu SFDC Campaign hinzufügen</td> 
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

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des **[!UICONTROL SFDC-Typs]** filtern, wobei der Operator auf &quot;[!UICONTROL ist nicht leer“ ]. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Denken Sie daran, dass diese automatischen Aktionen nur stattfinden, wenn sich der Lead derzeit nicht in [Salesforce.com befindet](https://salesforce.com){target="_blank"}
