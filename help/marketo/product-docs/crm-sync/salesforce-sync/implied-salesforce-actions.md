---
unique-page-id: 4719304
description: Implementierte Salesforce-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Implizite Salesforce-Aktionen
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Implizite Salesforce-Aktionen {#implied-salesforce-actions}

Wenn ein Salesforce-spezifischer Flussschritt ausgeführt wird, werden manchmal automatisch zusätzliche Schritte ausgeführt. Im Folgenden finden Sie die Regeln, damit Sie Folgendes wissen:

Diese Regeln gelten _, wenn sich die Person derzeit nicht in [Salesforce.com](https://Salesforce.com)_ als Kontakt oder Lead.

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

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe der **SFDC-Typ** Filtern Sie mit dem Operator, der auf &quot;ist nicht leer&quot;gesetzt ist. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Denken Sie daran, dass diese automatischen Aktionen nur stattfinden, wenn der Lead derzeit nicht in [Salesforce.com](https://salesforce.com)
