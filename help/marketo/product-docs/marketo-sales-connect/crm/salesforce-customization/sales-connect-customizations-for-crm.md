---
unique-page-id: 14745793
description: Sales Connect-Anpassungen für CRM - Marketo-Dokumente - Produktdokumentation
title: Sales Connect-Anpassungen für CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: dbf058714f6c4e6003c5a64d1048ac8a47931a0f
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 2%

---

# Sales Connect-Anpassungen für CRM {#sales-connect-customizations-for-crm}

Die Felder und Schaltflächen unten werden von der Metadaten-API im Salesforce CRM erstellt. Nach der Erstellung der Felder müssen Administratoren die Seitenlayouts in ihrem CRM-System konfigurieren, um sie verfügbar zu machen. Anweisungen [finden Sie hier](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Installieren von Anpassungen in Salesforce {#how-to-install-customizations-in-salesforce}

1. Klicken Sie in Sales Connect auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one.png)

1. Wählen Sie unter &quot;Admin Settings&quot;den Eintrag **Salesforce**.

   ![](assets/two.png)

1. Klicken Sie auf **Marketo Sales Connect-Anpassungen**.

   ![](assets/three.png)

1. Klicken Sie auf **Verbindung zu Salesforce herstellen**.

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

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Lokale Präsenz-ID des MSE-Aufrufs</td>
    <td>Als Benutzer können Sie bei Aufrufen über das MSE Phone "Lokale Präsenz"als Option wählen. Eingehende Aufrufe zeigen eine lokale Nummer für den Empfänger an.</td>
  </tr>
  <tr>
    <td>URL zur Aufzeichnung von MSE-Aufrufen</td>
    <td>Aufrufe können aufgezeichnet werden und hier wird ein Link für die Aufzeichnung protokolliert.</td>
  </tr>
  <tr>
    <td>MSE-Kampagne</td>
    <td>Protokollierungsname der MSE-Kampagne, der der Kontakt/Lead angehört.</td>
  </tr>
  <tr>
    <td>MSE-Kampagnen-URL</td>
    <td>Protokolliert die URL für die in MSE erstellte Kampagne. Wenn Sie auf diese Option klicken, wird die Kampagne in der MSE-Web-App geöffnet.</td>
  </tr>
  <tr>
    <td>Aktueller Schritt einer MSE-Kampagne</td>
    <td>Wenn ein Kontakt/Lead Teil einer Kampagne ist, protokolliert dieses Feld den Namen des Schritts, in dem sich der Lead/Kontakt derzeit befindet.</td>
  </tr>
  <tr>
    <td>Angezeigte MSE-E-Mail-Anlage</td>
    <td>Protokolliert Daten, wenn eine E-Mail mit einem Anhang gesendet und der Anhang vom Empfänger angezeigt wird.</td>
  </tr>
  <tr>
    <td>MSE-E-Mail angeklickt</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger auf einen Link in einer E-Mail klickt.</td>
  </tr>
  <tr>
    <td>MSE-E-Mail beantwortet</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger auf eine E-Mail antwortet.</td>
  </tr>
  <tr>
    <td>MSE Email Status</td>
    <td>Zeigt an, ob eine E-Mail gesendet/in Bearbeitung/abgestürzt wurde (das Tracking nicht zugestellter E-Mails hängt vom verwendeten Versandkanal ab).</td>
  </tr>
  <tr>
    <td>MSE Email Template</td>
    <td>Logs name of the MSE template that was used in the email sent to the lead/contact.</td>
  </tr>
  <tr>
    <td>URL der MSE-E-Mail-Vorlage</td>
    <td>Protokolliert die URL auf die in MSE erstellte Vorlage. Wenn Sie auf diese Option klicken, wird die Vorlage in der MSE-Web-App geöffnet.</td>
  </tr>
  <tr>
    <td>MSE Email URL</td>
    <td>Wenn Sie auf diese URL klicken, wird das Command Center in MSE geöffnet und die Registerkarte "People Detail View history"abgerufen, auf der Sie die gesendete E-Mail sehen können.</td>
  </tr>
  <tr>
    <td>Angezeigte MSE-E-Mail</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger eine E-Mail anzeigt.</td>
  </tr>
</tbody></table>

## Datenaggregations-Protokollierungsfelder {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Letzte Marketinginteraktion</td>
    <td>Letzte eingehende Interaktion vom Marketing.</td>
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
    <td>MSE - Letzter Marketing-Interaktionstyp</td>
    <td>Art der Interaktion.</td>
  </tr>
  <tr>
    <td>MSE - Letzte Aktivität nach Vertrieb</td>
    <td>Letzte ausgehende Aktivität, die vom Sales-Team durchgeführt wurde.</td>
  </tr>
  <tr>
    <td>MSE - Zuletzt geantwortet</td>
    <td>Letzte E-Mail-Antwort auf die E-Mail "Verkauf".</td>
  </tr>
  <tr>
    <td>MSE - Aktuelle Vertriebskampagne</td>
    <td>Protokollname der MSE-Kampagne, der der Lead/Kontakt angehört.</td>
  </tr>
  <tr>
    <td>MSE - Letzte Vertriebsinteraktion</td>
    <td>Letzte eingehende Interaktion aus dem Verkauf.</td>
  </tr>
  <tr>
    <td>MSE - Opt-out</td>
    <td>Opt-out-Feld.</td>
  </tr>
</tbody></table>

## Schaltflächen {#buttons}

<table><thead>
  <tr>
    <th>Schaltflächenname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE-E-Mail senden</td>
    <td>Senden Sie E-Mails zum Vertrieb aus Salesforce.</td>
  </tr>
  <tr>
    <td>Zu MSE-Kampagne hinzufügen</td>
    <td>Zu MSE-Kampagnen aus Salesforce hinzufügen.</td>
  </tr>
  <tr>
    <td>Push to MSE</td>
    <td>Push-Kontakt von Salesforce zu MSE.</td>
  </tr>
  <tr>
    <td>Aufruf mit MSE</td>
    <td>Führen Sie Verkaufsaufrufe von Salesforce aus durch.</td>
  </tr>
</tbody>
</table>

## Massenaktion - Schaltflächen {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Schaltflächenname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Zu MSE-Kampagne hinzufügen</td>
    <td>Zu MSE-Kampagnen aus Salesforce hinzufügen.</td>
  </tr>
  <tr>
    <td>Push to MSE</td>
    <td>Push-Kontakt von Salesforce zu MSE.</td>
  </tr>
</tbody>
</table>

## Benutzerhandbücher {#user-guides}

[Benutzerdefinierte MSE-Berichte in Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE für Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE für Salesforce-Blitze](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
