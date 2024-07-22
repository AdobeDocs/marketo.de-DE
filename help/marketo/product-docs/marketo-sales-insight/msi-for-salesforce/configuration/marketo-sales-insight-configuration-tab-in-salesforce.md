---
unique-page-id: 42762322
description: Registerkarte "Konfiguration von Marketo Sales Insight"in Salesforce - Marketo Docs - Produktdokumentation
title: Marketo Sales Insight-Konfigurationsregisterkarte in Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 4848676d423ff96c2e880819bc760b2f8dbbd094
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Marketo Sales Insight-Konfigurationsregisterkarte in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Betriebseinstellungen {#operational-settings}

Sie müssen diese Einstellung einrichten, um Sales Insight in SFDC verwenden zu können.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI verwendet sowohl die Soap- als auch die Rest-API
* Die Seite &quot;Sales Insight&quot;in Ihrem Marketo-Konto enthält zwei entsprechende Bereiche mit Soap- und Rest-API-Anmeldeinformationen, die Sie hier kopieren und einfügen können.
* Die Soap- und Rest-API verfügt über separate Zeitlimits, die Sie entsprechend den Anforderungen Ihres Unternehmens festlegen können. Die maximal zulässige Zeit beträgt 120 Sekunden
* Deaktivieren des Insights-Dashboards: Sie können REST-API-Anmeldeinformationen entfernen und nur die Soap-API verwenden. Dadurch wird die Registerkarte Insights Dashboard in allen MSI Visualisierungs-Bedienfeldern deaktiviert.

## MSI-Konfiguration {#msi-configuration}

Konfigurationen gelten für alle MSI-Benutzer und sind nicht profilspezifisch.

**Visualforce-Seiteneinstellungen**

* Aktivieren der Dropdown-Liste Aktion :
   * Möglichkeit, Marketo-E-Mail aus der Dropdown-Liste im Lead- und Kontakt-MSI-Layout auszublenden
   * Möglichkeit, die Optionen Zu Marketo-Campaign hinzufügen aus der Dropdown-Liste in Lead- und Kontakt-MSI-Layout auszublenden
* Anstehende Ereignisse: Möglichkeit, eingeladene Ereignisse, alle Ereignisse für Benutzer anzuzeigen oder diese Registerkarte vollständig auszublenden
* Kampagnen: Möglichkeit, alle E-Mail-Kampagnen anzuzeigen oder diesen Tab vollständig auszublenden
* Bevorstehende Kampagnen und Ereignisse laden: Möglichkeit, die Anzahl der REST-API-Aufrufe von Benutzern zu reduzieren, indem die Registerkarte &quot;Ereignisse und Kampagnen&quot;hinter einer On-Demand-Schaltfläche &quot;Bevorstehende Elemente laden&quot;platziert wird
* Registerkarteneinstellungen: Standardmäßig sind alle fünf Registerkarten verfügbar. Sie können die Reihenfolge der Registerkarten im Bereich Sales Insight auswählen. Dieselbe Reihenfolge gilt für alle Layouts (Lead, Kontakt, Konto, Chancen)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Globale Registerkarte &quot;Marketo&quot;**

* RSS-Feed aktiviert: Wenn diese Option aktiviert ist, können MSI-Benutzer ihren Lead-Feed in einem RSS-Feed anzeigen (zusätzlich zum Lead-Feed in Salesforce). Der RSS-Feed kann nur funktionieren, wenn die Funktion &quot;Token-Ablauf&quot;deaktiviert ist. Diese Einstellung wird auf Ihrer Marketo Sales Insight-Administrationsseite gesteuert.
* Debug-Modus für vielversprechende Kontakte
* Standardausblendung: Die Option, die Sie hier auswählen, ist die Anzahl der Tage, in denen eine der besten Wetten auf der Registerkarte &quot;Beste Wetten&quot;in Marketo ausgeblendet wird, wenn Sie auf das Symbol &quot;Ausblenden&quot;klicken
* Kontaktstatusfeld: Die Option, die Sie hier auswählen, ist der Wert, der in der Spalte Statuskopfzeile auf der Registerkarte Beste Betas in Marketo ausgefüllt wird.
* Live-Feed-Einstellungen: Die Option, nur Live-Feed (in den Bedienfeldern &quot;Lead&quot;, &quot;Kontakt&quot;, &quot;Konto&quot;und &quot;Chancen&quot;sowie auf der Seite &quot;Globale Marketo&quot;anzuzeigen), nur Lead-Feed (auf der globalen Seite von Marketo) oder sowohl Live- als auch Lead-Feed anzuzeigen.
* Registerkarteneinstellungen: Standardmäßig sind alle fünf Registerkarten verfügbar. Sie können die Reihenfolge der Registerkarten auf der globalen Marketo-Seite auswählen

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Beschränkungen**

* Aktivität (interessanter Moment, Web-Aktivität, E-Mail) ist standardmäßig auf 1000 gesetzt. E-Mail-Kampagnen und -Ereignisse sind standardmäßig auf 200 gesetzt
* Falls Sie bei Ihrer Organisation Probleme mit der Zeitüberschreitung bemerken, können Sie die Beschränkung

**Aktionseinstellungen**

* Marketo-E-Mail senden: Durch Aktivierung dieser Option erhalten alle Sales Insight-Benutzer Zugriff auf das Senden von E-Mails aus den Bereichen Lead, Kontakt, Konto, Chancen und der Registerkarte Beste Betas (Massenaktionen und Inline-Interaktion).
* Zu Marketo Campaign hinzufügen: Durch Aktivierung dieser Option können alle Sales Insight-Benutzer Kampagnen aus den Bereichen Lead, Kontakt, Konto, Chancen und der Registerkarte Beste Betas (Massenaktionen und Inline-Interaktion) hinzufügen.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Support-Einstellungen {#support-settings}

Wenn Sie dieses Kontrollkästchen aktivieren, wird die Debug-Protokollierung in Ihrer Salesforce-Instanz aktiviert. Es kann Ihnen bei der Fehlerbehebung helfen.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## Marketo Sales Insight zurücksetzen {#reset-marketo-sales-insight}

Wenn Sie sich dafür entscheiden, werden alle Ihre Konfigurationen in SFDC gelöscht und sie können nicht wiederhergestellt werden. Sie müssen alles erneut konfigurieren.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>Aktivieren Sie das Kontrollkästchen &quot;MSI-Aktionen aktivieren&quot;, es sei denn, Sie verwenden die Funktionen von Sales Insights-Aktionen .

>[!MORELIKETHIS]
>
>[Hinzufügen von Sales Insight-Zugriff zu Profilen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
