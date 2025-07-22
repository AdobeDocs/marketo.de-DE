---
unique-page-id: 7504051
description: Verwalten von Personendaten - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Personendaten
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 23%

---

# Verwalten von Personendaten {#manage-person-data}

Nutzen Sie Personendaten für die [!DNL Web Personalization], indem Sie die in Ihrer Segmentierung zu verwendenden Personenfelder auswählen.

1. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Wechseln Sie zu **[!UICONTROL Datenbank]**.

   ![](assets/account-settings-dropdown-database.jpg)

## Hinzufügen eines Felds „Neue Person“ {#adding-a-new-person-field}

1. Wählen Sie **Feld zum Hinzufügen** aus der Dropdown-Liste aus, um der Liste ein Personendatenfeld hinzuzufügen.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Ein neues Feld wird im Status Ausstehend hinzugefügt und kann bis zu 24 Stunden dauern, bis es aktiviert ist.

## Löschen eines Personenfelds {#deleting-a-person-field}

1. Klicken Sie auf das Löschsymbol ( ![—](assets/image2015-3-24-13-3a45-3a56.png)), um ein Feld aus der Liste zu entfernen. Klicken Sie **[!UICONTROL Ja]**, um zu bestätigen, dass Sie das Feld löschen möchten.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Verwalten von Personendatenfeldern**
   >
   >* Nur Personendatenfelder können einbezogen werden
   >* Sie können bis zu 30 Personendatenfelder hinzufügen
   >* Bis zum Aktivieren hinzugefügter neuer Felder können bis zu 24 Stunden vergehen
   >* Die maximal zulässige Länge der String-Typen ist 255 Zeichen
   >* Ausgeblendete Felder werden automatisch entfernt

<table> 
 <tbody> 
  <tr> 
   <th><p>REST-API-Name</p></th> 
   <th><p>SOAP-API-Name</p></th> 
   <th><p>Anzeigename</p></th> 
  </tr> 
  <tr> 
   <td><p>Abteilung</p></td> 
   <td><p>Abteilung</p></td> 
   <td><p>Abteilung</p></td> 
  </tr> 
  <tr> 
   <td><p>Titel</p></td> 
   <td><p>Titel</p></td> 
   <td><p>Jobtitel</p></td> 
  </tr> 
  <tr> 
   <td><p>Bewertung</p></td> 
   <td><p>Rating</p></td> 
   <td><p>Rating</p></td> 
  </tr> 
  <tr> 
   <td><p>LeadScore</p></td> 
   <td><p>LeadScore</p></td> 
   <td><p>Ergebnis</p></td> 
  </tr> 
  <tr> 
   <td><p>leadStatus</p></td> 
   <td><p>LeadStatus</p></td> 
   <td><p>Status</p></td> 
  </tr> 
  <tr> 
   <td><p>Priorität</p></td> 
   <td><p>Priorität</p></td> 
   <td><p>Priorität</p></td> 
  </tr> 
  <tr> 
   <td><p>leadRole</p></td> 
   <td><p>LeadRole</p></td> 
   <td><p>Rolle</p></td> 
  </tr> 
  <tr> 
   <td><p>Abgemeldet</p></td> 
   <td><p>Abbestellt</p></td> 
   <td><p>Abbestellt</p></td> 
  </tr> 
 </tbody> 
</table>

Die folgenden Lead-Felder sind für neue [!DNL Web Personalization]-Konten standardmäßig bereitgestellt:

>[!MORELIKETHIS]
>
>[Erstellen eines Segments mithilfe von Daten zu bekannten Personen](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
