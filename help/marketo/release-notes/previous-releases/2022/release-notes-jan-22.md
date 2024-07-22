---
description: Januar 2022 - Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Januar 2022 - Versionshinweise
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Januar 2022 - Versionshinweise {#release-notes-jan-22}

Die folgenden Funktionen sind in der Version vom 22. Januar enthalten. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden ab dem 21. Januar 2022 veröffentlicht, wobei jede Funktion schrittweise über die folgenden Wochen eingeführt wird (sofern nicht anders angegeben).****

## Erlebnis der nächsten Generation {#modern-ux}

* **Screens im Erlebnis der nächsten Generation aktualisiert**: Wir stellen zusätzliche, aktualisierte Bildschirme der nächsten Generation bereit, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, auf die über den Umschalter zugegriffen werden kann:

   * Asset-Details für Landingpages in Design Studio
   * Asset-Details der Landingpage in Marketingaktivitäten

## Microsoft Dynamics-Integration {#microsoft-dynamics-integration}

* **Synchronisierung des Feldtyps &quot;Multiselect-Optionssatz allgemein verfügbar&quot;**: Synchronisieren Sie den Feldtyp für Mehrfachauswahl in Microsoft Dynamics, um ihn in Smart-Listen und Smart-Kampagnen zu verwenden und so ein granulareres Zielgruppen-Targeting zu ermöglichen. Beispiele sind: Themen/Produkte von Interesse, bevorzugte Kommunikationsformen und mehr. Diese neue Synchronisierung ist für Microsoft Dynamics Version 9.X (einschließlich Dynamics 365 Online) verfügbar.

* **Server-zu-Server-Authentifizierung für Microsoft Dynamics 365 Online**: Für mehr Sicherheit unterstützen wir jetzt S2S (Server to Server to Server) als zusätzlichen Authentifizierungsmodus für den Marketo Engage-Synchronisierungsbenutzer in Azure Active Directory für den nicht interaktiven Zugriff auf Microsoft Dynamics 365 Online. Auf diese Weise können Sie eine Authentifizierung mit mehreren Faktoren verwenden, da alle Authentifizierungen und Anmeldungen auf OAuth basieren (nur Client-ID und Client-Geheimnis).

>[!NOTE]
>
>Der S2S-Modus basiert auf dem Anwendungsbenutzer und nicht auf dem lizenzierten Benutzer, wodurch die Verwendung einer zusätzlichen Lizenz gespeichert wird.

## Administration {#administration}

* **[Formularvalidierungsregeln](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Behalten Sie den Zustand Ihrer Datenbank bei, sodass Sie problematische oder unerwünschte E-Mail-Domänen daran hindern können, Marketo Engage-Formulare zu senden. Im Bereich &quot;Globale Formularvalidierungsregel&quot;können Administratoren eine Blockierungsliste definieren oder eine vordefinierte Liste freier Verbraucherdomänen aktivieren, um sie von Formularen zu blockieren.

* **[Sicherheit der Landingpage-Kopfzeile](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Administratoren können die Header für die strikte Transportsicherheit und X-Frame-Optionen auf ihren Landingpage-Domänen verwalten, um starke Sicherheitsanforderungen zu erzwingen.

**_Herausgabe während des gesamten Quartals_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## AEP Marketo Engage Destination Connector - Erstellen neuer Leads {#aep-marketo-engage-destination-connector}

Marketo Engage-Kunden, die auch Adobe Experience Platform (AEP) verwenden, können ihre Datenbank maximieren, indem sie netto-neue Personendatensätze über den AEP-Zielanschluss per Push in Marketo Engage von AEP übertragen können. Beim Senden von Zielgruppensegmenten von AEP an Marketo Engage können Personen innerhalb des Segments, die noch nicht in Ihrer Marketo Engage-Datenbank vorhanden sind, [automatisch hinzugefügt werden](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

**Sales Insight für Salesforce CRM**

* **Spalte &quot;Neuer Typ&quot;für die besten Betas**: Verkäufer erhalten schnellere Einblicke mit einer neuen Spalte mit der Bezeichnung &quot;Typ&quot;, um auf der Seite &quot;Beste Einsätze&quot;zwischen Leads und Kontakten zu unterscheiden.

* **Salesforce Platform-API-Update**: Als Reaktion auf Salesforce, Salesforce Platform-API-Versionen 21.0 bis 30.0 eingestellt hat, wurde das Sales Insight-Paket mit den neuesten APIs aktualisiert.

* **Aktualisiertes Branding**: Alle Sales Insight-Seiten werden aktualisiert, um sie an das Adobe-Branding anzupassen.

**Sales Insight für Microsoft Dynamics**

* **Aktualisiertes Kontolayout**: Verkäufer können eine kollektive Ansicht der wichtigsten Aktivitäten wie E-Mail-Aktivitäten, Web-Aktivitäten, interessante Momente und Bewertungsänderungen für alle Kontakte innerhalb eines Kontos erhalten.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Ergebnisse und Gründe aufrufen**: Verstehen und verfolgen Sie die ausgehenden Bemühungen Ihrer Verkaufsteams mit neuen, vollständig anpassbaren Aufrufergebnissen und Anrufbegründungsoptionen im Detail. Zusätzlich zu diesen neuen Feldern führen wir eine neue Governance ein, um die Anrufbegründung und Ergebnisauswahl zu erzwingen, während Verkäufer Aufrufe tätigen, eine neue Governance, um Anrufgründe und -ergebnisse zu aktivieren oder zu deaktivieren, und ein neues benutzerdefiniertes Feld &quot;Anrufgrund&quot;und &quot;Salesforce-Aktivität aufrufen&quot;für die Protokollierung von Daten in Salesforce. [Klicken Sie hier](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) , um mehr zu erfahren.

* **Anpassung der Details der Salesforce-Aktivität**: Erfassen Sie mehr Verkaufsaktivitäten und Aufgabendaten in Salesforce, indem Sie anpassen, welche Informationen zum Betrefffeld der Salesforce-Aufgabe hinzugefügt werden, wenn eine Verkaufsaktivität von Sales Connect aus bei Salesforce protokolliert wird. [Klicken Sie hier](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) , um mehr zu erfahren.

## Ankündigungen {#announcements}

* **Marketo Sky Deprecation**: Im März ist Marketo Sky nicht mehr verfügbar, da wir unsere Ressourcen auf die Bereitstellung des Benutzererlebnisses der nächsten Generation konzentrieren. Um den Zugriff auf Funktionen zu erhalten, die heute nur noch für Marketo Sky verfügbar sind, setzen wir Asset-Ablauf und Smart-Campaign-Prioritätsüberschreibungen im März in das allgemeine Erlebnis ein. [Klicken Sie hier](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) , um mehr zu erfahren.

* **Form Endpoints Deprecation**: Nicht unterstützte programmatische Formular-POSTs zum LeadCapture/save2-Endpunkt werden von Marketo Engage Forms zurückgewiesen. [Klicken Sie hier](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) , um mehr zu erfahren.

**Marketo Engage-Domänen - Sales Insight-Konfiguration**: Für Marketo Engage-Domänen, für die kein SSL-Zertifikat bereitgestellt wurde, und https:// schlagen Aufrufe mit einem SSL-Handshake-Fehler fehl. Daher werden diese Domänen abgestürzt sein. Daher können Sales Insight-Benutzer mit einer älteren Konfiguration, die auf eine dieser Domänen verweist, bei ihrer Lead-, Kontakt-, Konto-, Opportunity Panels- oder Marketo Global-Seite möglicherweise Systemberechnungsfehler feststellen. Wenn dieser Fehler auftritt, sollten Sie Ihre [Marketo Engage-Konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in Salesforce aktualisieren. Sie müssen lediglich die Marketo Engage-Anmeldeinformationen aktualisieren, die im Abschnitt &quot;Marketo Sales Insight-Konfiguration&quot;des Dokuments hervorgehoben sind.

**_Webinar zur Produktversion_**

[Marketo Engage-Release-Webinar vom Januar 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
