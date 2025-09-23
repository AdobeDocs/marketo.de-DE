---
unique-page-id: 4719294
description: Anpassen der Aktivitätssynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Anpassen der Aktivitätensynchronisierung
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 2%

---

# Anpassen der Aktivitätensynchronisierung {#customize-activities-sync}

Wenn Sie Marketo Sales Insight nicht verwenden, kann Marketo Engage Salesforce-Aktivitätsverlaufsdatensätze für bestimmte Ereignisse erstellen. So aktivieren Sie sie.

>[!NOTE]
>
>Die Salesforce-/Marketo Engage-Synchronisierung überträgt keine Aktivitäten an Salesforce, die stattgefunden haben, bevor die Person an Salesforce gepusht wurde.

1. Wechseln Sie zu **[!UICONTROL Admin]**.

   ![](assets/customize-activities-sync-1.png)

1. Klicken Sie auf **[!DNL Salesforce]** und dann auf **[!UICONTROL Synchronisierungsoptionen bearbeiten]**.

   ![](assets/two-1.png)

1. Aktivieren Sie die Kontrollkästchen neben den Aktivitäten, die Marketo an Salesforce pushen soll, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Nach der Aktivierung überträgt Marketo den Aktivitätsverlauf für drei Monate. Je nach Datenmenge (_kann mehrere Tage dauern_. Aktualisierungen, die während der ersten Push-Aktivitäten auftreten, können verzögert werden, bis die Synchronisierung der ersten Aktivitäten abgeschlossen ist.

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
   <td>[!UICONTROL ausgefülltes Formular]</td>
   <td>Beliebiges Marketo-Formular ausgefüllt</td>
  </tr>
  <tr>
   <td>[!UICONTROL zur Liste hinzugefügt]</td>
   <td><p>Flussschritt: wurde zu einer statischen Liste hinzugefügt</p></td>
  </tr>
  <tr>
   <td>[!UICONTROL E-Mail gesendet]</td>
   <td>Flussschritt: Es wurde eine E-Mail gesendet</td>
  </tr>
  <tr>
   <td>[!UICONTROL E-Mail zugestellt]</td>
   <td>Eine E-Mail erhalten (nicht zurückgesendet)</td>
  </tr>
  <tr>
   <td>[!UICONTROL E-Mail geöffnet]</td>
   <td>Geöffnete E-Mails (ohne Bilder zu blockieren)</td>
  </tr>
  <tr>
   <td>[!UICONTROL Link in E-Mail angeklickt]</td>
   <td>Auf einen Link in einer von Marketo gesendeten E-Mail geklickt</td>
  </tr>
  <tr>
   <td>[!UICONTROL aus Liste entfernt]</td>
   <td>Flussschritt: wurde aus einer statischen Liste entfernt</td>
  </tr>
  <tr>
   <td>[!UICONTROL Aus Fluss entfernen]</td>
   <td>Flussschritt: Aus Fluss entfernen</td>
  </tr>
  <tr>
   <td>[!UICONTROL Verkaufs-E-Mail gesendet]</td>
   <td>Eine E-Mail wurde über Marketo Sales Insight gesendet</td>
  </tr>
  <tr>
   <td>[!UICONTROL Verkaufs-E-Mail geöffnet]</td>
   <td>hat eine über Marketo Sales Insight gesendete E-Mail geöffnet</td>
  </tr>
  <tr>
   <td>[!UICONTROL Link in Verkaufs-E-Mail anklicken]</td>
   <td>Auf einen Link in einer über Marketo Sales Insight gesendeten E-Mail geklickt</td>
  </tr>
  <tr>
   <td>[!UICONTROL Verkaufs-E-Mail empfangen]</td>
   <td>Eine E-Mail wurde vom Vertriebsmitarbeiter im MSI Outlook-Plug-in empfangen und protokolliert.</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>„Erhaltene Verkaufs-E-Mail _bedeutet nicht_ Zustellung. Der Status Zugestellt wird für E-Mails, die über Sales Insight gesendet werden, nicht erfasst.

>[!TIP]
>
>Wenn Sie weitere Informationen zu Marketo in Salesforce erhalten möchten, lesen Sie unser [Produkt zu Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
