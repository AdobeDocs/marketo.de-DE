---
unique-page-id: 14745793
description: Sales Connect-Anpassungen für CRM - Marketo-Dokumente - Produktdokumentation
title: Sales Connect-Anpassungen für CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Sales Connect-Anpassungen für CRM {#sales-connect-customizations-for-crm}

Die Felder und Schaltflächen unten werden von der Metadaten-API in Salesforce CRM erstellt. Nach der Erstellung der Felder müssen Administratoren die Seitenlayouts in ihrem CRM-System konfigurieren, um sie verfügbar zu machen. Anweisungen finden Sie [hier](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Dies wirkt sich sowohl auf ToutApp- als auch auf Sales Connect-Kunden aus.

## Installieren von Anpassungen in Salesforce {#how-to-install-customizations-in-salesforce}

1. Klicken Sie in Sales Connect auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one.png)

1. Wählen Sie unter &quot;Admin Settings&quot;**Salesforce** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Marketo Sales Connect-Anpassungen**.

   ![](assets/three.png)

1. Klicken Sie auf **Mit Salesforce verbinden**.

   ![](assets/four.png)

1. Melden Sie sich bei Salesforce an.

   ![](assets/five.png)

## Salesforce-Anpassung aktualisieren {#update-salesforce-customization}

Aktualisierungen des Salesforce-Anpassungspakets umfassen Verbesserungen und Fehlerkorrekturen. Gehen Sie wie folgt vor, um zu überprüfen, ob Updates verfügbar sind oder um eine Aktualisierung durchzuführen.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen.**

1. Klicken Sie in der [Webanwendung](https://www.toutapp.com) auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Auf der Karte zur Anpassung von Sales Connect wird angezeigt, ob Updates verfügbar sind. Klicken Sie auf **Anpassungen aktualisieren**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Klicken Sie auf **Upgrade**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Warten Sie, bis die Updates installiert sind. Je nachdem, wie viele Versionsnummern Sie benötigen, variiert die Installationszeit.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Nach Abschluss des Vorgangs zeigt Ihre Karte an, dass Ihre Anpassungen an Sales Connect aktuell sind.

![](assets/sales-connect-customizations-for-crm-11.png)

## Benutzerdefinierte Aktivitätsfelder {#custom-activity-fields}

Marketo erkennt die Erstellung der neuen Felder und führt dann eine einmalige Aufstockung der Daten, eine erneute Zuordnung und eine fortlaufende Synchronisierung der Werte nur in den **neuen** -Feldern durch. Alte Felder werden nicht aktualisiert.

| **Feldname** | **Beschreibung** |
|---|---|
| Lokale Präsenz-ID des MSE-Aufrufs | Als Benutzer können Sie bei Aufrufen über das MSE Phone &quot;Lokale Präsenz&quot;als Option wählen. Eingehende Aufrufe zeigen eine lokale Nummer für den Empfänger an. |
| URL zur Aufzeichnung von MSE-Aufrufen | Aufrufe können aufgezeichnet werden und hier wird ein Link für die Aufzeichnung protokolliert. |
| MSE-Kampagne | Protokollierungsname der MSE-Kampagne, der der Kontakt/Lead angehört. |
| MSE-Kampagnen-URL | Protokolliert die URL für die in MSE erstellte Kampagne. Wenn Sie auf diese Option klicken, wird die Kampagne in der MSE-Web-App geöffnet. |
| Aktueller Schritt einer MSE-Kampagne | Wenn ein Kontakt/Lead Teil einer Kampagne ist, protokolliert dieses Feld den Namen des Schritts, in dem sich der Lead/Kontakt derzeit befindet. |
| Angezeigte MSE-E-Mail-Anlage | Protokolliert Daten, wenn eine E-Mail mit einem Anhang gesendet und der Anhang vom Empfänger angezeigt wird. |
| MSE-E-Mail angeklickt | Protokolliert ein Häkchen, wenn der Empfänger auf einen Link in einer E-Mail klickt. |
| MSE-E-Mail beantwortet | Protokolliert ein Häkchen, wenn der Empfänger auf eine E-Mail antwortet. |
| MSE Email Status | Zeigt an, ob eine E-Mail gesendet/in Bearbeitung/abgestürzt wurde (das Tracking nicht zugestellter E-Mails hängt vom verwendeten Versandkanal ab). |
| MSE Email Template | Logs name of the MSE template that was used in the email sent to the lead/contact. |
| URL der MSE-E-Mail-Vorlage | Protokolliert die URL auf die in MSE erstellte Vorlage. Wenn Sie auf diese Option klicken, wird die Vorlage in der MSE-Web-App geöffnet. |
| MSE Email URL | Wenn Sie auf diese URL klicken, wird das Command Center in MSE geöffnet und die Registerkarte &quot;People Detail View history&quot;abgerufen, auf der Sie die gesendete E-Mail sehen können. |
| Angezeigte MSE-E-Mail | Protokolliert ein Häkchen, wenn der Empfänger eine E-Mail anzeigt. |

## Datenaggregations-Protokollierungsfelder {#roll-up-logging-fields}

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
   <td>MSE - Letzte Marketinginteraktion</td> 
   <td>Letzte eingehende Interaktion vom Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Datum der letzten Marketing-Interaktion</td> 
   <td>Zeitstempel der Interaktion vom Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Letzte Marketing Engagement Desc</td> 
   <td>Beschreibung der Interaktion.</td> 
  </tr> 
  <tr> 
   <td>MSE - Letzte Marketinginteraktion - Source</td> 
   <td>Source der Marketinginteraktion.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzter Marketing-Interaktionstyp</td> 
   <td colspan="1">Art der Interaktion.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzte Aktivität nach Vertrieb<br></td> 
   <td colspan="1">Letzte ausgehende Aktivität, die vom Sales-Team durchgeführt wurde.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Zuletzt geantwortet</td> 
   <td colspan="1">Letzte E-Mail-Antwort auf die E-Mail "Verkauf".</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Aktuelle Vertriebskampagne</td> 
   <td colspan="1">Protokollname der MSE-Kampagne, der der Lead/Kontakt angehört.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Letzte Vertriebsinteraktion</td> 
   <td colspan="1">Letzte eingehende Interaktion aus dem Verkauf. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Opt-out</td> 
   <td colspan="1">Opt-out-Feld.</td> 
  </tr> 
 </tbody> 
</table>

## Schaltflächen {#buttons}

| **Schaltflächenname** | **Beschreibung** |
|---|---|
| MSE-E-Mail senden | Senden Sie E-Mails zum Vertrieb von Salesforce. |
| Zu MSE-Kampagne hinzufügen | Fügen Sie zu MSE-Kampagnen aus Salesforce hinzu. |
| Push to MSE | Push-Kontakt von Salesforce zu MSE. |
| Aufruf mit MSE | Führen Sie Verkaufsaufrufe von Salesforce durch. |

## Massenaktion - Schaltflächen {#bulk-action-buttons}

| **Schaltflächenname** | **Beschreibung** |
|---|---|
| Zu MSE-Kampagne hinzufügen | Fügen Sie zu MSE-Kampagnen aus Salesforce hinzu. |
| Push to MSE | Push-Kontakt von Salesforce zu MSE. |

## Benutzerhandbücher {#user-guides}

[MSE Benutzerspezifische Berichte in Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE für Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE für Salesforce-Blitze](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
