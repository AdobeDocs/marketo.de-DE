---
unique-page-id: 7504051
description: Erfahren Sie mehr über die Verwaltung von Personendaten in Marketo Engage, einschließlich der Verwaltung von Personendaten „manage-person-data“. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Verwalten von Personendaten
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
TQID: https://experienceleague.adobe.com/rIiC-JXLkaMByk7GizVOcCEcUHN8AL-8Hy66-U2GZhs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 24%

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
   <td><p>Job-Titel</p></td>
  </tr>
  <tr>
   <td><p>Bewertung</p></td>
   <td><p>Bewertung</p></td>
   <td><p>Bewertung</p></td>
  </tr>
  <tr>
   <td><p>LeadScore</p></td>
   <td><p>LeadScore</p></td>
   <td><p>Bewertung</p></td>
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
   <td><p>Hat sich abgemeldet</p></td>
   <td><p>Abbestellt</p></td>
  </tr>
 </tbody>
</table>

Die folgenden Lead-Felder sind für neue [!DNL Web Personalization]-Konten standardmäßig bereitgestellt:

>[!MORELIKETHIS]
>
>[Erstellen eines Segments mithilfe von Daten zu bekannten Personen](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
