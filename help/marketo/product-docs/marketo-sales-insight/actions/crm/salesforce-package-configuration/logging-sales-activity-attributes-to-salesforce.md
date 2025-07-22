---
description: Protokollieren von Attributen der Verkaufsaktivität in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Protokollieren von Attributen der Verkaufsaktivität in Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 10%

---

# Protokollieren von Attributen der Verkaufsaktivität in [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

Der Salesforce-Administrator kann [!DNL Salesforce] manuell benutzerdefinierte Aktivitätsfelder hinzufügen.

1. Klicken Sie in Ihrem [!DNL Salesforce] auf **[!UICONTROL Setup]**.

1. Suchen Sie im Schnellsuchfeld nach „Benutzerdefinierte Aktivitätsfelder“ und klicken Sie darauf.

1. Klicken Sie auf **[!UICONTROL Neu]**.

1. Wählen Sie basierend auf der unten stehenden Tabelle den Datentyp für das Feld aus, das Sie hinzufügen möchten, und klicken Sie auf **[!UICONTROL Weiter]**.

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
  <td>[!UICONTROL Aufrufergebnisse]</td>
  <td>motosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Aufrufgründe]</td>
  <td>motosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Verkaufsaufruf Lokale Präsenz-ID]</td>
  <td>MSE_CALL_LOCAL_PRESENCE_ID</td>
  <td>mse_call_local_presence_id__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo-URL für die Aufzeichnung von Verkaufsanrufen]</td>
  <td>MSE_CALL_RECORDING</td>
  <td>MSE_CALL_RECORDING__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo-Vertriebskampagne]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign - Aktueller Schritt]</td>
  <td>mse_current_campaign_step</td>
  <td>MSE_CURRENT_CAMPAIGN_STEP__C</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebskampagnen-URL]</td>
  <td>MSE_CAMPAIGN_DETAILS_LINK</td>
  <td>MSE_CAMPAIGN_DETAILS_LINK__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Anhang zum Marketo-Verkauf angezeigt]</td>
  <td>MSE_PRESENTATION_VIEWED</td>
  <td>MSE_PRESENTATION_VIEWED__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail zum Verkauf von Marketo angeklickt]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail zum Vertrieb von Marketo beantwortet]</td>
  <td>MSE_Replied</td>
  <td>MSE_REPLIED__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Status Marketo-Verkauf]</td>
  <td>MSE_EMAIL_STATUS</td>
  <td>MSE_EMAIL_STATUS__c</td>
  <td>Text</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Vorlage für Vertrieb in Marketo]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>MSE_Details</td>
  <td>MSE_DETAILS__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail zum Verkauf von Marketo angezeigt]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Kontrollkästchen</td>
  <td></td>
 </tr>
</table>
