---
unique-page-id: 4719294
description: Aktivitäten anpassen - Synchronisierung - Marketing-Dokumente - Produktdokumentation
title: Synchronisieren von Aktivitäten anpassen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Synchronisieren von Aktivitäten anpassen {#customize-activities-sync}

Wenn Sie [Sales Insight](http://docs.marketo.com/display/DOCS/Marketo+Sales+Insight)nicht verwenden, kann Marketo für bestimmte Ereignis Salesforce-Aktivitäten-Verlaufsberichte erstellen. So können sie aktiviert werden.

1. Gehen Sie zu **Admin. **

   ![](assets/admin.png)

1. Klicken Sie auf **Salesforce** und dann auf **Edit Sync Options**.

   ![](assets/two-1.png)

1. Markieren Sie die Kästchen neben den Aktivitäten, die Marketo an Salesforce senden soll, und klicken Sie auf **Speichern**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Nach der Aktivierung wird Marketo die Aktivität von drei Monaten in die Geschichte einbringen. Je nach Datenmenge kann *dies mehrere Tage dauern*. Updates, die während des Push-Vorgangs zu den ersten Aktivitäten auftreten, können bis zum Abschluss der Synchronisierung der ersten Aktivitäten verschoben werden.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Aktivität</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ausgefülltes Formular</td> 
   <td>Ausfüllen von Markierungsformularen</td> 
  </tr> 
  <tr> 
   <td>Zur Liste hinzugefügt</td> 
   <td><p>Flussschritt: Wurde einer statischen Liste hinzugefügt</p></td> 
  </tr> 
  <tr> 
   <td>Email gesendet</td> 
   <td>Flussschritt: Wurde eine E-Mail gesendet</td> 
  </tr> 
  <tr> 
   <td>Ausgelieferte E-Mail</td> 
   <td>Eine E-Mail erhalten (nicht abgespielt)</td> 
  </tr> 
  <tr> 
   <td>Email geöffnet</td> 
   <td>Öffnen einer E-Mail (ohne Blockieren von Bildern)</td> 
  </tr> 
  <tr> 
   <td>Link in E-Mail angeklickt</td> 
   <td>Klicken Sie auf einen Link in einer E-Mail von Marketo</td> 
  </tr> 
  <tr> 
   <td>Aus Liste entfernt</td> 
   <td>Flussschritt: Wurde aus einer statischen Liste entfernt</td> 
  </tr> 
  <tr> 
   <td>Aus Fluss entfernen</td> 
   <td>Flussschritt: Aus Fluss entfernen</td> 
  </tr> 
  <tr> 
   <td>E-Mail-Versand</td> 
   <td>Wurde per E-Mail über Marketing an Sales Insight gesendet</td> 
  </tr> 
  <tr> 
   <td>Verkaufsemail geöffnet</td> 
   <td>Öffnen einer E-Mail, die über MarketingTo Sales Insight gesendet wurde</td> 
  </tr> 
  <tr> 
   <td>Link in Verkaufs-E-Mail</td> 
   <td>Klicken Sie auf einen Link in einer E-Mail, die über MarketingTo Sales Insight gesendet wurde.</td> 
  </tr> 
  <tr> 
   <td>E-Mail erhalten</td> 
   <td>Eine E-Mail wurde vom Vertriebsmitarbeiter im MSI Outlook Plugin empfangen und protokolliert</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Erinnerung**
>
>
>&quot;E-Mail beim Vertrieb erhalten&quot;bedeutet **nicht** , dass sie zugestellt wird. Der Status &quot;Ausgeliefert&quot;wird nicht für E-Mails erfasst, die über Sales Insight gesendet werden.

>[!TIP]
>
>Wenn Sie mehr Marketo-Informationen in Salesforce erhalten möchten, schauen Sie sich unser [Produkt Marketing Insight](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) an.

