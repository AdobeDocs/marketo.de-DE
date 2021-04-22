---
unique-page-id: 4719294
description: Synchronisieren von Aktivitäten - Marketo Docs - Produktdokumentation
title: Synchronisieren von Aktivitäten anpassen
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Aktivitäten anpassen Synchronisieren {#customize-activities-sync}

Wenn Sie Marketo Sales Insight nicht verwenden, kann Marketo für bestimmte Ereignis Salesforce-Aktivitäten-Historikdatensätze erstellen. So können sie aktiviert werden.

1. Gehen Sie zu **Admin**.

   ![](assets/admin.png)

1. Klicken Sie auf **Salesforce** und dann auf **Synchronisierungsoptionen bearbeiten**.

   ![](assets/two-1.png)

1. Markieren Sie die Kästchen neben den Aktivitäten, die Marketo an Salesforce senden soll, und klicken Sie auf **Speichern**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Nach der Aktivierung wird Marketo die Aktivität von drei Monaten in die Geschichte einbringen. Je nach Datenmenge kann es mehrere Tage dauern, bis _abgeschlossen ist._ Updates, die während des Push-Vorgangs zu den ersten Aktivitäten auftreten, können bis zum Abschluss der Synchronisierung der ersten Aktivitäten verschoben werden.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Aktivitätstyp</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ausgefülltes Formular</td> 
   <td>Ausfüllen von Marketo-Formularen</td> 
  </tr> 
  <tr> 
   <td>Der Liste hinzugefügt</td> 
   <td><p>Flussschritt: Wurde einer statischen Liste hinzugefügt</p></td> 
  </tr> 
  <tr> 
   <td>E-Mail gesendet</td> 
   <td>Flussschritt: Wurde eine E-Mail gesendet</td> 
  </tr> 
  <tr> 
   <td>E-Mail übermittelt</td> 
   <td>Eine E-Mail erhalten (nicht abgespielt)</td> 
  </tr> 
  <tr> 
   <td>E-Mail geöffnet</td> 
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
   <td>Aus Flow entfernen</td> 
   <td>Flussschritt: Aus Fluss entfernen</td> 
  </tr> 
  <tr> 
   <td>Vertriebs-E-Mail gesendet</td> 
   <td>Wurde per E-Mail an Marketo Sales Insight gesendet</td> 
  </tr> 
  <tr> 
   <td>Vertriebs-E-Mail geöffnet</td> 
   <td>Öffnen einer E-Mail, die über Marketo Sales Insight gesendet wurde</td> 
  </tr> 
  <tr> 
   <td>Link in Verkaufs-E-Mail</td> 
   <td>Klicken Sie auf einen Link in einer E-Mail, die über Marketo Sales Insight gesendet wurde.</td> 
  </tr> 
  <tr> 
   <td>Vertriebs-E-Mail empfangen</td> 
   <td>Eine E-Mail wurde vom Vertriebsmitarbeiter im MSI Outlook Plugin empfangen und protokolliert</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-Mail zum Verkauf erhalten&quot; bedeutet **nicht** mittlere Zustellung. Der Status &quot;Ausgeliefert&quot;wird nicht für E-Mails erfasst, die über Sales Insight gesendet werden.

>[!TIP]
>
>Wenn Sie weitere Marketo-Informationen in Salesforce erhalten möchten, sehen Sie sich unser [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) Produkt an.
