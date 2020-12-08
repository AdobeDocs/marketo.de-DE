---
unique-page-id: 4719304
description: Implizierte Salesforce-Aktionen - Marketing Docs - Produktdokumentation
title: Implizierte Salesforce-Aktionen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Implizierte Salesforce-Aktionen {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Wenn ein Salesforce-spezifischer Flussschritt ausgeführt wird, werden manchmal zusätzliche Schritte automatisch ausgeführt. Hier sind die Regeln, Sie wissen also:

Diese Regeln gelten *dann, wenn die Person derzeit nicht als Kontakt oder Interessent in [Salesforce.com](http://Salesforce.com)* ist.

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
   <td>Person mit<br>SFDCAdd mit SFDC-Kampagne synchronisieren</td> 
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

Sie können SFDC-Datensätze in einer Smart-Liste mithilfe des **SFDC-Type** -Filters herausfiltern, wobei der Operator auf &quot;ist nicht leer&quot;eingestellt ist. Alle SFDC-Datensätze haben in diesem Feld einen Wert.

Beachten Sie, dass diese automatischen Aktionen nur stattfinden, wenn der Interessent derzeit nicht in [Salesforce.com aufgeführt ist.](http://Salesforce.com)

Die Salesforce-Synchronisierung ist cool, nicht wahr?
