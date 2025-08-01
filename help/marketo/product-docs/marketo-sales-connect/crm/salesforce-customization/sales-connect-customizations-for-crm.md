---
unique-page-id: 14745793
description: '[!DNL Sales Connect] für CRM - Marketo-Dokumente - Produktdokumentation'
title: '[!DNL Sales Connect] für CRM'
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 2%

---

# [!DNL Sales Connect] für CRM {#sales-connect-customizations-for-crm}

Die folgenden Felder und Schaltflächen werden von der Metadaten-API in Salesforce CRM erstellt. Nachdem die Felder erstellt wurden, müssen Administratoren die Seiten-Layouts in ihrem CRM konfigurieren, um sie verfügbar zu machen. Anweisungen [finden Sie hier](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Installieren von Anpassungen in [!DNL Salesforce] {#how-to-install-customizations-in-salesforce}

1. Klicken Sie [!DNL Sales Connect] auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/one.png)

1. Wählen [!UICONTROL  unter „Admin] die Option **[!UICONTROL Salesforce]**.

   ![](assets/two.png)

1. Klicken Sie auf **[!UICONTROL Marketo Sales Engage-Anpassungen]**.

   ![](assets/three.png)

1. Klicken Sie **[!UICONTROL Mit Salesforce verbinden]**.

   ![](assets/four.png)

1. Melden Sie sich bei [!DNL Salesforce] an.

   ![](assets/five.png)

## [!DNL Salesforce] aktualisieren {#update-salesforce-customization}

Die Aktualisierungen des Pakets zur [!DNL Salesforce] enthalten Verbesserungen und Fehlerbehebungen. Gehen Sie wie folgt vor, um zu überprüfen, ob Updates verfügbar sind oder um ein Update durchzuführen.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich.**

1. Klicken Sie in [Web-Anwendung](https://www.toutapp.com) auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Klicken [!UICONTROL  unter „Admin-]&quot; auf **[!UICONTROL Salesforce]**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Auf der Karte Anpassung [!DNL Sales Connect] wird angezeigt, ob Aktualisierungen verfügbar sind. Klicken Sie **[!UICONTROL Anpassungen aktualisieren]**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Warten Sie, bis die Updates installiert sind. Je nachdem, wie viele Versionsnummern Sie benötigen, variiert die Installationszeit.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Nach der Fertigstellung zeigt Ihre Karte „Ihre Sales Connect-Anpassungen sind auf dem neuesten Stand.“

![](assets/sales-connect-customizations-for-crm-11.png)

## Benutzerdefinierte Aktivitätsfelder {#custom-activity-fields}

Marketo erkennt die Erstellung der neuen Felder und führt dann eine einmalige Aufstockung der Daten, eine Neuzuordnung und eine fortlaufende Synchronisierung von Werten nur in die **neuen** Felder durch. Alte Felder werden nicht aktualisiert.

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Lokale Präsenz-ID des SMS-Aufrufs</td>
    <td>Als Benutzer können Sie bei Anrufen vom MSE-Telefon die Option Lokale Präsenz als Option wählen. Bei eingehenden Anrufen wird eine lokale Nummer für den Empfänger angezeigt.</td>
  </tr>
  <tr>
    <td>URL für die Aufzeichnung von SMS-Aufrufen</td>
    <td>Anrufe können aufgezeichnet werden und ein Link für die Aufzeichnung wird hier protokolliert.</td>
  </tr>
  <tr>
    <td>MSE-Kampagne</td>
    <td>Loggt den Namen der SMS-Kampagne, der der Kontakt/Lead angehört.</td>
  </tr>
  <tr>
    <td>MSE-Kampagnen-URL</td>
    <td>Protokolliert die URL für die in MSE erstellte Kampagne. Wenn Sie darauf klicken, wird die Kampagne in der MSE-Web-App geöffnet.</td>
  </tr>
  <tr>
    <td>Aktueller Schritt der SMS-Kampagne</td>
    <td>Wenn ein Kontakt/Lead Teil einer Kampagne ist, wird in diesem Feld der Name des Schritts protokolliert, in dem sich der Lead/Kontakt derzeit befindet.</td>
  </tr>
  <tr>
    <td>MSE-E-Mail-Anhang angesehen</td>
    <td>Protokolliert Daten, wenn eine E-Mail mit einer Anlage gesendet und die Anlage vom Empfänger angezeigt wird.</td>
  </tr>
  <tr>
    <td>E-Mail-Adresse angeklickt</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger auf einen Link in einer E-Mail klickt.</td>
  </tr>
  <tr>
    <td>SMS-E-Mail geantwortet</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger auf eine E-Mail antwortet.</td>
  </tr>
  <tr>
    <td>SMS-E-Mail-Status</td>
    <td>Zeigt an, ob eine E-Mail gesendet/in Bearbeitung/nicht zugestellt wurde (Tracking von nicht zugestellten E-Mails hängt vom verwendeten Versandkanal ab).</td>
  </tr>
  <tr>
    <td>MSE-E-Mail-Vorlage</td>
    <td>Loggt den Namen der MSE-Vorlage, die in der an den Lead/Kontakt gesendeten E-Mail verwendet wurde.</td>
  </tr>
  <tr>
    <td>MSE-E-Mail-Vorlagen-URL</td>
    <td>Protokolliert die URL in der in MSE erstellten Vorlage. Wenn Sie darauf klicken, wird die Vorlage in der MSE-Web-App geöffnet.</td>
  </tr>
  <tr>
    <td>MSE Email URL</td>
    <td>Wenn Sie auf diese URL klicken, wird das Command Center in MSE geöffnet und die Registerkarte „Personen-Detailansicht - Verlauf“ aufgerufen, auf der die gesendete E-Mail zu sehen ist.</td>
  </tr>
  <tr>
    <td>MSE-E-Mail angesehen</td>
    <td>Protokolliert ein Häkchen, wenn der Empfänger eine E-Mail anzeigt.</td>
  </tr>
</tbody></table>

## Rollout-Protokollfelder {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Letzte Marketing-Interaktion</td>
    <td>Letzte eingehende Interaktion aus Marketing.</td>
  </tr>
  <tr>
    <td>MSE - Datum des letzten Marketing-Engagements</td>
    <td>Zeitstempel der Interaktion mit Marketing.</td>
  </tr>
  <tr>
    <td>MSE - Beschreibung der letzten Marketing-Interaktion</td>
    <td>Beschreibung des Engagements.</td>
  </tr>
  <tr>
    <td>MSE - Letzte Marketing-Interaktion Source</td>
    <td>Source der Marketing-Interaktion.</td>
  </tr>
  <tr>
    <td>MSE - Typ der letzten Marketing-Interaktion</td>
    <td>Art der Interaktion.</td>
  </tr>
  <tr>
    <td>MSE - Letzte Aktivität nach Verkauf</td>
    <td>Letzte ausgehende Aktivität, die vom Sales-Team ausgeführt wurde.</td>
  </tr>
  <tr>
    <td>MSE - Zuletzt geantwortet</td>
    <td>Letzte E-Mail Antwort auf Verkaufs-E-Mail.</td>
  </tr>
  <tr>
    <td>MSE - Aktuelle Verkaufskampagne</td>
    <td>Loggt den Namen der SMS-Kampagne, der der Lead/Kontakt angehört.</td>
  </tr>
  <tr>
    <td>MSE - Letztes Vertriebsvorhaben</td>
    <td>Letzte eingehende Interaktion vom Verkauf.</td>
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
    <td>SMS-E-Mail senden</td>
    <td>Senden Sie Verkaufs-E-Mails von Salesforce.</td>
  </tr>
  <tr>
    <td>Zur MSE-Kampagne hinzufügen</td>
    <td>Zu MSE-Kampagnen aus Salesforce hinzufügen.</td>
  </tr>
  <tr>
    <td>Push an MSE</td>
    <td>Push-Kontakt von Salesforce zu MSE.</td>
  </tr>
  <tr>
    <td>Anruf mit MSE</td>
    <td>Führen Sie Verkaufsanrufe von Salesforce aus.</td>
  </tr>
</tbody>
</table>

## Massenaktion-Schaltflächen {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Schaltflächenname</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Zur MSE-Kampagne hinzufügen</td>
    <td>Zu MSE-Kampagnen aus Salesforce hinzufügen.</td>
  </tr>
  <tr>
    <td>Push an MSE</td>
    <td>Push-Kontakt von Salesforce zu MSE.</td>
  </tr>
</tbody>
</table>

## Benutzerhandbücher {#user-guides}

[Benutzerdefinierte MSE-Berichte in Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE für Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE für Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
