---
unique-page-id: 4719304
description: Implizite Salesforce-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Implizierte Salesforce-Aktionen
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 26%

---

# Implizierte Salesforce-Aktionen {#implied-salesforce-actions}

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
   <td>Hinzufügen zu SFDC-Kampagne</td>
   <td>Synchronisieren von Personen mit SFDC</td>
  </tr>
  <tr>
   <td>Ändern des Status in SFDC-Kampagne</td>
   <td>Person mit SFDC synchronisieren<br> Zu SFDC Campaign hinzufügen</td>
  </tr>
  <tr>
   <td>Ändern von Eigentümerin bzw. Eigentümer</td>
   <td><p>Synchronisieren von Personen mit SFDC</p></td>
  </tr>
  <tr>
   <td>Konvertieren von Person</td>
   <td><p>Synchronisieren von Personen mit SFDC</p></td>
  </tr>
  <tr>
   <td>Erstellen von Aufgaben</td>
   <td>Synchronisieren von Personen mit SFDC</td>
  </tr>
 </tbody>
</table>

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des **[!UICONTROL SFDC-Typs]** filtern, wobei der Operator auf &quot;[!UICONTROL ist nicht leer“ ]. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Denken Sie daran, dass diese automatischen Aktionen nur stattfinden, wenn sich der Lead derzeit nicht in [Salesforce.com befindet](https://salesforce.com){target="_blank"}
