---
unique-page-id: 4719294
description: Aktivitätensynchronisierung anpassen - Marketo-Dokumente - Produktdokumentation
title: Aktivitätensynchronisierung anpassen
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Aktivitätensynchronisierung anpassen {#customize-activities-sync}

Wenn Sie Marketo Sales Insight nicht verwenden, kann Marketo Engage für bestimmte Ereignisse Salesforce Activity History Records erstellen. So können sie aktiviert werden.

1. Wechseln Sie zu **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicken Sie auf **[!DNL Salesforce]** und dann auf **[!UICONTROL Synchronisierungsoptionen bearbeiten]**.

   ![](assets/two-1.png)

1. Aktivieren Sie die Kontrollkästchen neben den Aktivitäten, die Marketo an Salesforce senden soll, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Nach der Aktivierung wird Marketo den Aktivitätsverlauf über einen Zeitraum von drei Monaten nachverfolgen. Je nach Datenmenge kann _es mehrere Tage dauern, bis_ abgeschlossen ist. Aktualisierungen, die während der ersten Aktivitäts-Push-Benachrichtigung auftreten, können bis zum Abschluss der ersten Aktivitätensynchronisierung verzögert sein.

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
   <td>Marketo-Formular ausfüllen</td> 
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
   <td>Eine E-Mail erhalten (nicht abgeschnitten)</td> 
  </tr> 
  <tr> 
   <td>E-Mail geöffnet</td> 
   <td>Öffnen einer E-Mail (ohne Bilder zu blockieren)</td> 
  </tr> 
  <tr> 
   <td>Link in E-Mail angeklickt</td> 
   <td>Auf einen Link in einer von Marketo gesendeten E-Mail geklickt</td> 
  </tr> 
  <tr> 
   <td>Aus Liste entfernt</td> 
   <td>Flussschritt: wurde aus einer statischen Liste entfernt</td> 
  </tr> 
  <tr> 
   <td>Aus Flow entfernen</td> 
   <td>Flussschritt: Aus Fluss entfernen</td> 
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail gesendet</td> 
   <td>Wurde über Marketo Sales Insight per E-Mail versendet</td> 
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail geöffnet</td> 
   <td>Öffnen einer E-Mail, die über Marketo Sales Insight gesendet wurde</td> 
  </tr> 
  <tr> 
   <td>Link in Verkaufs-E-Mail</td> 
   <td>Auf einen Link in einer E-Mail geklickt, die über Marketo Sales Insight gesendet wurde</td> 
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail empfangen</td> 
   <td>Eine E-Mail wurde vom Vertriebsmitarbeiter im MSI Outlook-Plugin empfangen und protokolliert</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-Mail zum Verkauf empfangen&quot;bedeutet nicht _, dass gesendet wird._ Der Status Zugestellt wird nicht für E-Mails erfasst, die über Sales Insight gesendet werden.

>[!TIP]
>
>Wenn Sie weitere Marketo-Informationen in Salesforce erhalten möchten, sehen Sie sich unser Produkt [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} an.
