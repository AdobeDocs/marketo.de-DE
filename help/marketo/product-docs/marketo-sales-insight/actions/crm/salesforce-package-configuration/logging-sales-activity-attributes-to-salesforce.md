---
description: Protokollieren von Attributen der Verkaufsaktivität in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Protokollieren von Attributen der Verkaufsaktivität in Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 30%

---

# Protokollieren von Attributen der Verkaufsaktivität in Salesforce {#logging-sales-activity-attributes-to-salesforce}

Der Salesforce-Administrator kann Salesforce manuell benutzerdefinierte Aktivitätsfelder hinzufügen.

1. Klicken Sie in Ihrem Salesforce-Konto auf **Setup**.

1. Suchen Sie im Schnellsuchfeld nach „Benutzerdefinierte Aktivitätsfelder“ und klicken Sie darauf.

1. Klicken Sie auf **Neu**.

1. Wählen Sie basierend auf der unten stehenden Tabelle den Datentyp für das Feld aus, das Sie hinzufügen möchten, und klicken Sie auf **Weiter**.

1. Geben Sie den Feldnamen und den Titel ein, der dem hinzuzufügenden Feld entspricht.

Beschreibung der einzelnen Spalten in der folgenden Tabelle:

* **Feldbezeichnung**: Feldname, der in der Benutzeroberfläche angezeigt wird (dieser Name kann angepasst werden, um die Lesbarkeit durch Ihr Team zu verbessern)
* **Feldname**: Technischer Name des Felds (stellen Sie sicher, dass der eingegebene Feldname mit dem Feldnamen in der folgenden Tabelle übereinstimmt)
* **API-Name**: Technischer Name des Felds für die API (stellen Sie sicher, dass der eingegebene API-Name mit dem API-Namen in der folgenden Tabelle übereinstimmt)
* **Datentyp**: Feldtyp
* **Size**: Größe des Textfelds

<table>
 <tr>
  <th>Feldbezeichnung</th>
  <th>Feldname</th>
  <th>API-Name</th>
  <th>Datentyp</th>
  <th>Größe</th>
 </tr>
  <tr>
  <td>Aufrufergebnisse</td>
  <td>motosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Gründe für den Anruf</td>
  <td>motosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Lokale Präsenz-ID des Marketo Sales-Anrufs</td>
  <td>MSE_CALL_LOCAL_PRESENCE_ID</td>
  <td>mse_call_local_presence_id__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Aufnahme-URL des Marketo Sales-Anrufs</td>
  <td>MSE_CALL_RECORDING</td>
  <td>MSE_CALL_RECORDING__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales-Kampagne</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Aktueller Schritt der Marketo Sales-Kampagne</td>
  <td>mse_current_campaign_step</td>
  <td>MSE_CURRENT_CAMPAIGN_STEP__C</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL der Marketo Sales-Kampagne</td>
  <td>MSE_CAMPAIGN_DETAILS_LINK</td>
  <td>MSE_CAMPAIGN_DETAILS_LINK__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Angesehener Anhang der Marketo Sales-E-Mail</td>
  <td>MSE_PRESENTATION_VIEWED</td>
  <td>MSE_PRESENTATION_VIEWED__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Angeklickte Marketo Sales-E-Mail</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Beantwortete Marketo Sales-E-Mail</td>
  <td>MSE_Replied</td>
  <td>MSE_REPLIED__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>Status der Marketo Sales-E-Mail</td>
  <td>MSE_EMAIL_STATUS</td>
  <td>MSE_EMAIL_STATUS__c</td>
  <td>Text</td>
  <td></td>
 </tr>
 <tr>
  <td>Vorlage für Marketo Sales-E-Mail</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL der Vorlage für Marketo Sales-E-Mail</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL der Marketo Sales-E-Mail</td>
  <td>MSE_Details</td>
  <td>MSE_DETAILS__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Angesehene Marketo Sales-E-Mail</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
</table>
