---
unique-page-id: 4719304
description: Implementierte Salesforce-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Implizite Salesforce-Aktionen
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 21%

---

# Implizite Salesforce-Aktionen {#implied-salesforce-actions}

Wenn ein Salesforce-spezifischer Flussschritt ausgeführt wird, werden manchmal automatisch zusätzliche Schritte ausgeführt. Im Folgenden finden Sie die Regeln, damit Sie Folgendes wissen:

Diese Regeln gelten, wenn sich die Person derzeit nicht in [Salesforce.com](https://Salesforce.com){target="_blank"} als Kontakt oder Lead befindet.

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
   <td>Person mit SFDC synchronisieren<br>Zu SFDC Campaign hinzufügen</td> 
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

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des Filters **[!UICONTROL SFDC-Typ]** herausfiltern, wobei der Operator auf &quot;ist nicht leer&quot;festgelegt ist. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Denken Sie daran, dass diese automatischen Aktionen nur stattfinden, wenn der Lead derzeit nicht in [Salesforce.com](https://salesforce.com){target="_blank"} enthalten ist.
