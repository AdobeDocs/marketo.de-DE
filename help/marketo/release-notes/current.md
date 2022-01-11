---
description: Aktuelle Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: f00d43080136dd986a6d81d6bc8102cdaf788b4c
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 2%

---

# Versionshinweise: Januar 2022 {#release-notes-jan-22}

Die folgenden Funktionen sind in der Version vom 22. Januar enthalten. Informieren Sie sich in Ihrer Adobe Marketo Engage Edition über die Verfügbarkeit von Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden veröffentlicht auf **21. Januar 2022**.

## Erlebnis der nächsten Generation {#next-generation-experience}

* **Aktualisierte Screens im Erlebnis der nächsten Generation**: Wir stellen zusätzliche, aktualisierte Bildschirme der nächsten Generation bereit, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, auf die über einen Umschalter zugegriffen werden kann:

   * Asset-Details für Landingpages in Design Studio
   * Asset-Details der Landingpage in Marketingaktivitäten

## Microsoft Dynamics-Integration {#microsoft-dynamics-integration}

* **Synchronisierung des Feldtyps &quot;Multiselect-Optionssatz&quot;allgemein verfügbar**: Synchronisieren Sie den Feldtyp für Mehrfachauswahl in Microsoft Dynamics, um ihn in Smart-Listen und Smart-Kampagnen für ein präziseres Zielgruppen-Targeting zu verwenden. Beispiele sind: Themen/Produkte von Interesse, bevorzugte Kommunikationsformen und mehr. Diese neue Synchronisierung ist für Microsoft Dynamics Version 9.X (einschließlich Dynamics 365 Online) verfügbar.

* **Server-zu-Server-Authentifizierung für Microsoft Dynamics 365 Online**: Aus Sicherheitsgründen unterstützen wir jetzt Server-to-Server (S2S) als zusätzlichen Authentifizierungsmodus für den Marketo Engage-Synchronisierungsbenutzer auf Azure Active Directory für den nicht interaktiven Zugriff auf Microsoft Dynamics 365 Online. Auf diese Weise können Sie eine Authentifizierung mit mehreren Faktoren verwenden, da alle Authentifizierungen und Anmeldungen auf OAuth basieren (nur Client-ID und Client-Geheimnis).

>[!NOTE]
>
>Der S2S-Modus basiert auf dem Anwendungsbenutzer und nicht auf dem lizenzierten Benutzer, wodurch die Verwendung einer zusätzlichen Lizenz gespeichert wird.

## Administration {#administration}

* **Formular-Validierungsregeln**: Warten Sie den Zustand Ihrer Datenbank, sodass Sie problematische oder unerwünschte E-Mail-Domains daran hindern können, Marketo Engage-Formulare zu senden. Im Bereich &quot;Globale Formularvalidierungsregel&quot;können Administratoren eine Blockierungsliste definieren oder eine vordefinierte Liste freier Verbraucherdomänen aktivieren, um sie von Formularen zu blockieren.

* **Sicherheit der Landingpage-Kopfzeile**: Administratoren können Header für strikte Transport-Sicherheit und X-Frame-Optionen auf ihren Landingpage-Domänen verwalten, um starke Sicherheitsanforderungen zu erzwingen.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## AEP Marketo Engage Destination Connector - Erstellen neuer Leads {#aep-marketo-engage-destination-connector}

Marketo Engage-Kunden, die auch die Adobe Experience Platform (AEP) verwenden, können ihre Datenbank maximieren, indem sie netto-neue Personendatensätze über den AEP-Ziel-Connector in Marketo Engage übertragen können. Beim Senden von Zielgruppensegmenten von AEP an Marketo Engage werden Personen innerhalb des Segments, die noch nicht in Ihrer Marketo Engage-Datenbank vorhanden sind, automatisch hinzugefügt.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

**Sales Insight für Salesforce CRM**

* **Spalte &quot;Neuer Typ&quot;für die besten Betas**: Verkäufer erhalten schnellere Einblicke mit einer neuen Spalte mit der Bezeichnung &quot;Typ&quot;, um auf der Seite &quot;Best Bets&quot;zwischen Leads und Kontakten zu unterscheiden.

* **Salesforce Platform-API-Update**: Als Reaktion auf die Einstellung der Salesforce Platform API-Versionen 21.0 bis 30.0 von Salesforce wurde das Sales Insight-Paket mit den neuesten APIs aktualisiert.

* **Aktualisiertes Branding**: Alle Sales Insight-Seiten werden aktualisiert, um sie an das Adobe-Branding anzupassen.

**Sales Insight für Microsoft Dynamics**

* **Aktualisiertes Kontolayout**: Verkäufer können einen kollektiven Überblick über die wichtigsten Aktivitäten erhalten, z. B.: E-Mail-Aktivitäten, Web-Aktivitäten, interessante Momente und Bewertungen von Änderungen für alle Kontakte innerhalb eines Kontos.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Ergebnisse und Gründe von Aufrufen**: Machen Sie sich mit den ausgehenden Bemühungen Ihrer Vertriebsteams mit neuen, vollständig anpassbaren Anrufergebnissen und Anrufbegründungsoptionen vertraut und verfolgen Sie sie detaillierter. Zusätzlich zu diesen neuen Feldern führen wir eine neue Governance ein, um die Anrufbegründung und Ergebnisauswahl zu erzwingen, während Verkäufer Aufrufe tätigen, eine neue Governance, um Anrufgründe und -ergebnisse zu aktivieren oder zu deaktivieren, und ein neues benutzerdefiniertes Feld &quot;Anrufgrund&quot;und &quot;Salesforce-Aktivität aufrufen&quot;für die Protokollierung von Daten in Salesforce. [Klicken Sie hier](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812), um mehr zu erfahren.

* **Anpassung der Salesforce-Aktivitätsdetails**: Erfassen Sie mehr Verkaufsaktivitäten und Aufgabendaten in Salesforce, indem Sie anpassen, welche Informationen zum Aufgabensubjekt Salesforce hinzugefügt werden, wenn eine Verkaufsaktivität von Sales Connect aus bei Salesforce protokolliert wird. [Klicken Sie hier](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819), um mehr zu erfahren.

## Ankündigungen {#announcements}

* **Marketo Sky Sunset**: Am 11. März wird Marketo Sky nicht mehr verfügbar sein, da wir unsere Ressourcen auf die Bereitstellung des Benutzererlebnisses der nächsten Generation konzentrieren. Um den Zugriff auf Funktionen zu erhalten, die heute nur noch für Marketo Sky verfügbar sind, setzen wir Asset-Ablauf und Smart-Campaign-Prioritätsüberschreibungen im März in das allgemeine Erlebnis ein.

* **Einstellung von Formularendpunkten**: Nicht unterstützte programmatische Formular-POSTs an den Endpunkt &quot;leadCapture/save2&quot;werden von Marketo Engage Forms abgelehnt. [Klicken Sie hier](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631), um mehr zu erfahren.

* **E-Mail-Überprüfung**: Ab dieser Version werden bei Marketo Engage-Abonnements &quot;Nur Nicht-API&quot;-Benutzer E-Mail-Adressen verifizieren. Für vom Verzeichnisdienst authentifizierte Benutzer werden ihre E-Mails automatisch überprüft, wenn ihr Abonnement mit E-Mail-Überprüfung aktiviert ist. Die E-Mail-Überprüfung für Benutzer, die die Funktion &quot;Dialogfeld für einladende Benutzer anmelden&quot;verwenden oder für die Abonnements, die über eine einzelne E-Mail mit mehreren Benutzern innerhalb des Abonnements verfügen, wird verzögert und fällt mit der Einstellung der Funktion im März zusammen.

* **Dialogfeld &quot;Benutzer einladen&quot;anmelden**: Im März wird die vorhandene optionale Funktion &quot;Anmelden im Dialogfeld &quot;Benutzer einladen&quot;eingestellt. Die Funktion &quot;Anmeldung im Dialogfeld &quot;Benutzer einladen&quot;wird durch die Funktion &quot;Universelle ID&quot;überschrieben, die für die bevorstehende Adobe der Identity Management-Systemintegration erforderlich ist und im August 2021 für alle Abonnements aktiviert wurde. Aufgrund der veralteten Version zwingt Marketo Engage, nur einen Benutzer pro E-Mail-Adresse innerhalb eines Abonnements zuzuordnen.

**Marketo Engage-Domänen - Konfiguration von Sales Insight**: Bei Marketo Engage-Domänen, für die kein SSL-Zertifikat bereitgestellt wurde, und https:// schlagen Aufrufe mit einem SSL-Handshake-Fehler fehl. Daher werden diese Domänen abgestürzt sein. Daher können Sales Insight-Benutzer mit einer älteren Konfiguration, die auf eine dieser Domänen verweist, bei ihrer Lead-, Kontakt-, Konto-, Opportunity Panels- oder Marketo Global-Seite möglicherweise Systemberechnungsfehler feststellen. Wir empfehlen Ihnen, Ihre [Marketo Engage-Konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in Salesforce , wenn dieser Fehler auftritt. Sie müssen nur die Marketo Engage-Anmeldeinformationen aktualisieren, die im Abschnitt &quot;Marketo Sales Insight-Konfiguration&quot;des Dokuments hervorgehoben sind.

**_Webinar zur Produktversion_**

Treten Sie uns am 27. Januar 2022 um 9:00 Uhr PT / 23:00 Uhr ET für eine [Live-Webinar](https://engage.marketo.com/2022_January_Release_Webinar_RegistrationPage.html) von unserem Produktteam gehostet, wo Sie erfahren können, wie Sie alle aktuellen Produktinnovationen nutzen können.
