---
description: Protokollieren von Attributen zu Verkaufsaktivitäten in Salesforce - Marketo Docs - Produktdokumentation
title: Protokollieren von Attributen für Verkaufsaktivitäten in Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 29%

---

# Protokollieren von Attributen für Verkaufsaktivitäten in Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce-Administrator kann Salesforce manuell benutzerdefinierte Aktivitätsfelder hinzufügen.

1. Klicken Sie in Ihrem Salesforce-Konto auf **Einrichten**.

1. Suchen Sie im Schnellsuchfeld nach &quot;Benutzerdefinierte Aktivitätsfelder&quot;und klicken Sie darauf.

1. Klicken Sie auf **Neu**.

1. Wählen Sie Datentyp aus, der dem Feld entspricht, das Sie basierend auf der Tabelle unten hinzufügen möchten, und klicken Sie auf **Weiter**.

1. Geben Sie den Feldnamen und die Beschriftung für das hinzuzufügende Feld ein.

Beschreibung der einzelnen Spalten in der unten stehenden Tabelle:

* **Feldbezeichnung**: In der Benutzeroberfläche angezeigter Feldname (dieser Name kann angepasst werden, um die Lesbarkeit durch Ihr Team zu verbessern)
* **Feldname**: Technischer Name des Felds (vergewissern Sie sich, dass der eingegebenen Feldname mit dem Feldnamen in der Tabelle unten übereinstimmt)
* **API-Name**: Technischer Name des Felds für die API (vergewissern Sie sich, dass der von Ihnen eingegebene API-Name mit dem API-Namen in der unten stehenden Tabelle übereinstimmt)
* **Datentyp**: Feldtyp
* **Größe**: Größe des Textfelds

<table>
 <tr>
  <th>Feldbezeichnung</th>
  <th>Feldname</th>
  <th>API-Name</th>
  <th>Datentyp</th>
  <th>Größe</th>
 </tr>
  <tr>
  <td>Ergebnisse der Aufrufe</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result_c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Gründe für Aufrufe</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason_c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Lokale Präsenz-ID des Marketo Sales-Anrufs</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Aufnahme-URL des Marketo Sales-Anrufs</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales-Kampagne</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign_c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Aktueller Schritt der Marketo Sales-Kampagne</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step_c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL der Marketo Sales-Kampagne</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Angesehener Anhang der Marketo Sales-E-Mail</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed_c_c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Angeklickte Marketo Sales-E-Mail</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked_c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Beantwortete Marketo Sales-E-Mail</td>
  <td>MSE_Response</td>
  <td>MSE_Replied_c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Status der Marketo Sales-E-Mail</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status_c</td>
  <td>Text</td>
  <td></td>
 </tr>
 <tr>
  <td>Vorlage für Marketo Sales-E-Mail</td>
  <td>MSE_Template</td>
  <td>MSE_Template_c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL der Vorlage für Marketo Sales-E-Mail</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL der Marketo Sales-E-Mail</td>
  <td>MSE_Details</td>
  <td>MSE_Details_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Angesehene Marketo Sales-E-Mail</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed_c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
</table>
