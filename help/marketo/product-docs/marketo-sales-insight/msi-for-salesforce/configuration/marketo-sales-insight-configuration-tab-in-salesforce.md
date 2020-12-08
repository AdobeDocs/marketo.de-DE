---
unique-page-id: 42762322
description: Registerkarte "Konfiguration von Marketo Sales Insight"in Salesforce - Marketo Docs - Produktdokumentation
title: Registerkarte "Konfiguration von Marketo Sales Insight" in Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Registerkarte &quot;Konfiguration von Marketo Sales Insight&quot; in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Operative Einstellungen {#operational-settings}

Sie müssen dies einrichten, um mit Sales Insight in SFDC Beginn zu erhalten.

![](assets/one.png)

* MSI verwendet SOAP- und Rest-API
* Die Seite &quot;Sales Insight&quot;in Ihrem Marketing-Konto verfügt über zwei zugehörige Bedienfelder mit Seife- und Rest-API-Anmeldeinformationen, die Sie hier kopieren und einfügen können.
* Die SOAP- und REST-API verfügt über separate Timeouts, die Sie je nach Bedarf Ihres Unternehmens festlegen können. Die maximal zulässige Zeit beträgt 120 Sekunden
* Insight-Dashboard deaktivieren: Sie können die Rest-API-Anmeldeinformationen entfernen und nur die SOAP-API verwenden. Dadurch wird die Registerkarte &quot;Insight-Dashboard&quot;in allen MSI-Visualforce-Bedienfeldern deaktiviert.

## MSI-Konfiguration {#msi-configuration}

Konfigurationen gelten für alle MSI-Benutzer und sind nicht spezifisch für Profil.

**Einstellungen für die Registerkarte &quot;Marketing&quot;**

* Best Bets-Debug-Modus
* Standardausblenden - Die Option, die Sie hier auswählen, ist die Anzahl der Tage, an denen eine beste Wette im Register Beste Wetten in Marketo ausgeblendet wird, wenn Sie auf das Symbol &quot;Ausblenden&quot; klicken
* Kontaktstatusfeld - Die hier gewählte Option ist der Wert, der in der Spalte Statuskopfzeile auf der Registerkarte Beste Bets in Marketing ausgefüllt wird
* Registerkarteneinstellungen - Alle 5 Registerkarten sind standardmäßig verfügbar. Sie können die Reihenfolge der Registerkarten auf der Seite &quot;Marketo global&quot;auswählen

**Visualforce-Seiteneinstellungen**

* Aktion-Dropdown aktivieren:

   * Möglichkeit zum Ausblenden von &quot;Send&quot;-E-Mail von Dropdown im &quot;Lead- und Kontakt-MSI-Layout&quot;
   * Möglichkeit, Optionen für Hinzufügen bis zur Kampagne von Marketing aus der Dropdown-Liste im Lead- und Kontakts-MSI-Layout auszublenden

* Anstehende Ereignisse: Möglichkeit, eingeladene Ereignis, alle Ereignis für Benutzer oder diese Registerkarte vollständig auszublenden
* Anstehende Kampagnen: Möglichkeit, alle E-Mail-Kampagnen anzuzeigen oder diese Registerkarte vollständig auszublenden
* Registerkarteneinstellungen - Alle 5 Registerkarten sind standardmäßig verfügbar. Alle 5 Registerkarten sind standardmäßig verfügbar. Sie können die Reihenfolge der Registerkarten im Bereich Sales Insight auswählen. Die gleiche Bestellung gilt für alle Layouts (Lead, Kontakt, Konto, Gelegenheit)

![](assets/two.png)

**Beschränkungen**

* Aktivität (Interessanter Moment, Web-Aktivität, E-Mail) ist standardmäßig auf 1000 eingestellt. E-Mail-Kampagnen und -Ereignis sind standardmäßig auf 200 eingestellt
* Falls Sie Probleme mit der Zeitüberschreitung auf Ihrer Organisation feststellen, können Sie die Beschränkung

## Zurücksetzen von Marketing auf Sales Insight {#reset-marketo-sales-insight}

Wenn Sie sich dafür entscheiden, werden alle Konfigurationen im SFDC gelöscht und können nicht wiederhergestellt werden. Sie müssen alles erneut konfigurieren.

![](assets/three.png)

