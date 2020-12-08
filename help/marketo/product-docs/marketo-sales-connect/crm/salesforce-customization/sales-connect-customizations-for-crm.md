---
unique-page-id: 14745793
description: Sales Connect-Anpassungen für CRM - Marketing-Dokumente - Produktdokumentation
title: Sales Connect-Anpassungen für CRM
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# Sales Connect-Anpassungen für CRM {#sales-connect-customizations-for-crm}

Die folgenden Felder und Schaltflächen werden von der Metadaten-API in Salesforce CRM erstellt. Nachdem die Felder erstellt wurden, müssen Administratoren die Seitenlayouts in ihrem CRM-System konfigurieren, um sie verfügbar zu machen. Anweisungen finden Sie [hier](http://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Dies betrifft sowohl ToutApp- als auch Sales Connect-Kunden.

## Installation von Anpassungen in Salesforce {#how-to-install-customizations-in-salesforce}

1. Klicken Sie in Sales Connect auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/one.png)

1. Wählen Sie unter &quot;Admin-Einstellungen&quot;die Option **Salesforce**.

   ![](assets/two.png)

1. Klicken Sie auf **Marketing Connect-Anpassungen**.

   ![](assets/three.png)

1. Klicken Sie auf **Mit Salesforce** verbinden.

   ![](assets/four.png)

1. Melden Sie sich bei Salesforce an.

   ![](assets/five.png)

## Benutzerdefinierte Aktivitäten {#custom-activity-fields}

Marketo erkennt die Erstellung der neuen Felder und führt dann eine einmalige Aufstockung der Daten, eine Neuzuordnung und eine fortlaufende Synchronisierung der Werte nur in die **neuen** Felder durch. Alte Felder werden nicht aktualisiert.

| **Feldname** | **Beschreibung** |
|---|---|
| Lokale Präsenz-ID für MSE-Aufruf | Als Benutzer können Sie &quot;Lokale Präsenz&quot;als Option wählen, wenn Sie über das MSE Phone anrufen. Bei eingehenden Anrufen wird eine lokale Nummer für den Empfänger angezeigt. |
| MSE-Aufrufungs-URL | Anrufe können aufgezeichnet werden und ein Link für die Aufzeichnung wird hier protokolliert. |
| MSE-Kampagne | Logs name of the MSE Kampagne the Contact/Lead is member of. |
| MSE-Kampagne-URL | Protokolliert die URL zur Kampagne, die in MSE erstellt wurde. Wenn Sie auf diese Schaltfläche klicken, wird die Kampagne in der MSE-Webanwendung geöffnet. |
| Aktueller Schritt zur MSE-Kampagne | Wenn ein Kontakt/Interessent zu einer Kampagne gehört, protokolliert dieses Feld den Namen des Schritts, auf dem der Interessent/Kontakt aktuell ist. |
| Angezeigte MSE-E-Mail-Anlage | Protokolliert Daten, wenn eine E-Mail mit einer Anlage gesendet und die Anlage vom Empfänger angezeigt wird. |
| MSE-E-Mail angeklickt | Protokolliert ein Häkchen, wenn der Empfänger auf einen Link in einer E-Mail klickt. |
| Antwort auf MSE-E-Mail | Protokolliert ein Häkchen, wenn der Empfänger auf eine E-Mail antwortet. |
| MSE-E-Mail-Status | Zeigt an, ob eine E-Mail gesendet/in Bearbeitung/abgespielt wird (die Verfolgung von abgesetzten E-Mails hängt vom verwendeten Versand-Kanal ab). |
| MSE-E-Mail-Vorlage | Protokollname der MSE-Vorlage, die in der an den Interessenten/Kontakt gesendeten E-Mail verwendet wurde. |
| URL der MSE-E-Mail-Vorlage | Protokolliert die URL zur Vorlage, die in MSE erstellt wurde. Durch Klicken auf diese Option wird die Vorlage in der MSE-Webanwendung geöffnet. |
| MSE-E-Mail-URL | Wenn Sie auf diese URL klicken, wird das Command Center in MSE geöffnet und die Registerkarte &quot;Ansicht der Personendaten&quot;abgerufen, auf der Sie die gesendete E-Mail sehen können. |
| Angezeigte MSE-E-Mail | Protokolliert ein Häkchen, wenn der Empfänger eine E-Mail Ansicht. |

## Datenaggregations-Protokollfelder {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Feldname</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Letzter Marketingeinsatz</td> 
   <td>Letzte eingehende Interaktion aus Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Letztes Marketingbindungsdatum</td> 
   <td>Zeitstempel der Interaktion vom Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Letzter Marketing-Einsatz-Desc</td> 
   <td>Beschreibung des Einsatzes.</td> 
  </tr> 
  <tr> 
   <td>MSE - Letzte Marketingeinsatzquelle</td> 
   <td>Quelle der Marketing-Interaktion.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzter Marketingeinsatztyp</td> 
   <td colspan="1">Art der Interaktion.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzte Aktivität nach Vertrieb<br></td> 
   <td colspan="1">Letzte ausgehende Aktivität durch das Vertriebsteam.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Zuletzt geantwortet</td> 
   <td colspan="1">Letzte E-Mail-Antwort auf die E-Mail von Vertrieb.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Kampagne des aktuellen Verkaufs</td> 
   <td colspan="1">Logs name of the MSE Kampagne the lead/contact is member of.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzter Vertriebseinsatz</td> 
   <td colspan="1">Letzte eingehende Interaktion von Vertrieb. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Opt-out</td> 
   <td colspan="1">Abmeldefeld.</td> 
  </tr> 
 </tbody> 
</table>

## Schaltflächen {#buttons}

| **Schaltflächenname** | **Beschreibung** |
|---|---|
| MSE-E-Mail senden | Senden Sie Verkaufs-E-Mails von Salesforce. |
| hinzufügen zur MSE-Kampagne | hinzufügen zu MSE-Kampagnen von Salesforce. |
| In MSE verschieben | Kontaktieren Sie Salesforce zu MSE. |
| Aufruf mit MSE | Treffen Sie Verkaufsanrufe von Salesforce. |

## Schaltflächen für Massenaktionen {#bulk-action-buttons}

| **Schaltflächenname** | **Beschreibung** |
|---|---|
| hinzufügen zur MSE-Kampagne | hinzufügen zu MSE-Kampagnen von Salesforce. |
| In MSE verschieben | Kontaktieren Sie Salesforce zu MSE. |

## Benutzerhandbücher {#user-guides}

[MSE Custom Reports in Salesforce](http://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE für Salesforce](http://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE für Salesforce-Blitz](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

## Verwandte Videos {#related-videos}

**Installation von Anpassungen in Salesforce**`<iframe width="630" height="470" src="//play.vidyard.com/YEPWYBfFEa4nKCo2F6bKKc.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>` ** Die Vorteile der Verwendung von Anpassungen in Salesforce**
`<iframe width="630" height="470" src="//play.vidyard.com/4PzSDb6o8Qg8WbvBsq8wJD.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`