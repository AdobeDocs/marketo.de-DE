---
description: Januar 2022 - Versionshinweise zu Marketo - Produktdokumentation
title: Januar 2022 - Versionshinweise
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Versionshinweise: Januar 2022 {#release-notes-jan-22}

Die folgenden Funktionen sind in der Version vom Januar 2022 enthalten. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden ab dem 21. **2022 veröffentlicht** wobei in den folgenden Wochen für jede Funktion ein schrittweiser Rollout erfolgt (sofern nicht anders angegeben).

## Erlebnis der nächsten Generation {#modern-ux}

* **Aktualisierter Screens im Erlebnis der nächsten Generation**: Wir bieten zusätzliche, aktualisierte Bildschirme im Erlebnis der nächsten Generation, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, die über einen Umschalter zugänglich sind:

   * Asset-Details für Landingpages in Design Studio
   * Asset-Details für Landingpages in Marketing-Aktivitäten

## Microsoft Dynamics-Integration {#microsoft-dynamics-integration}

* **Synchronisierung des Feldtyps für Mehrfachauswahl-Optionssätze allgemein verfügbar**: Synchronisieren Sie den Feldtyp für Mehrfachauswahl-Optionssätze aus Microsoft Dynamics, um ihn in Smart-Listen und Smart-Kampagnen für eine detailliertere Zielgruppenbestimmung zu nutzen. Beispiele sind: Themen/Produkte, die von Interesse sind, bevorzugte Kommunikationsformen und mehr. Diese neue Synchronisierung ist für Microsoft Dynamics Version 9.x verfügbar (einschließlich Dynamics 365 Online).

* **Server-zu-Server-Authentifizierung für Microsoft Dynamics 365 Online**: Für erhöhte Sicherheit unterstützen wir jetzt Server-zu-Server (S2S) als zusätzlichen Authentifizierungsmodus für den Marketo Engage-Synchronisierungsbenutzer in Azure Active Directory für den nicht interaktiven Zugriff auf Microsoft Dynamics 365 Online. Auf diese Weise können Sie die Multi-Faktor-Authentifizierung verwenden, da alle Authentifizierungen und Anmeldungen auf OAuth basieren (nur Client-ID und Client-Geheimnis).

>[!NOTE]
>
>Der S2S-Modus basiert auf dem Anwendungsbenutzer und nicht auf dem lizenzierten Benutzer, wodurch die Verwendung einer zusätzlichen Lizenz eingespart wird.

## Administration {#administration}

* **[Formularvalidierungsregeln](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Pflegen Sie den Zustand Ihrer Datenbank, indem Sie problematische oder unerwünschte E-Mail-Domains am Senden von Marketo Engage-Formularen hindern. Im Bedienfeld Globale Formularvalidierungsregel können Admins eine Blockierungsliste definieren oder eine vordefinierte Liste kostenloser Verbraucher-Domains aktivieren, die aus Formularen blockiert werden sollen.

* **[Kopfzeilensicherheit der Landingpage](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Administratoren können die Kopfzeilen „Strenge Transportsicherheit“ und „X-Frame-Optionen“ in den Domains der Landingpage verwalten, um strenge Sicherheitsanforderungen durchzusetzen.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## AEP Marketo Engage-Ziel-Connector - Erstellen neuer Leads {#aep-marketo-engage-destination-connector}

Marketo Engage-Kunden, die auch die Adobe Experience Platform (AEP) verwenden, können ihre Datenbank optimieren, indem sie neue Personendatensätze von AEP über den AEP-Ziel-Connector per Push in Marketo Engage übertragen. Beim Senden von Zielgruppensegmenten von AEP zu Marketo Engage können Personen innerhalb des Segments, die noch nicht in Ihrer Marketo Engage-[ vorhanden sind, automatisch hinzugefügt ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

**Sales Insight für Salesforce CRM**

* **Neue Typ-Spalte für Best**: Verkäufer erhalten schnellere Einblicke mit einer neuen Spalte mit der Bezeichnung „Typ“, um auf der Seite „Best Bets“ zwischen Leads und Kontakten zu unterscheiden.

* **Salesforce Platform-API-Aktualisierung**: Als Reaktion auf die Einstellung der Salesforce Platform-API-Versionen 21.0 bis 30.0 durch Salesforce wurde das Sales-Insight-Paket mit den neuesten APIs aktualisiert.

* **Aktualisiertes Branding**: Alle Sales Insight-Seiten werden aktualisiert, damit sie mit dem Adobe-Branding übereinstimmen.

**Sales Insight für Microsoft Dynamics**

* **Aktualisiertes Konto-Layout**: Verkäufer können sich einen Überblick über die wichtigsten Aktivitäten verschaffen, wie z. B. E-Mail-Aktivitäten, Web-Aktivitäten, interessante Momente und Bewertungsänderungen für alle Kontakte innerhalb eines Kontos.

## Sales Connect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Anrufergebnisse und -gründe**: Verstehen und verfolgen Sie die ausgehenden Bemühungen Ihrer Vertriebsteams detaillierter mit neuen, vollständig anpassbaren Anrufergebnis- und Anrufgrund-Optionen. Zusätzlich zu diesen neuen Feldern führen wir neue Governance ein, um die Auswahl der Anrufgründe und -ergebnisse zu erzwingen, während die Verkäufer Anrufe tätigen, neue Governance, um Anrufgründe und -ergebnisse zu aktivieren oder zu deaktivieren, und ein neues benutzerdefiniertes Feld für Anrufgrund und Anrufergebnis-Salesforce-Aktivität , um Daten in Salesforce zu protokollieren. [Hier klicken](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) um mehr zu erfahren.

* **Anpassung der Salesforce-Aktivitätsdetails**: Erfassen Sie mehr Daten zu Verkaufsaktivitäten und Aufgaben in Salesforce, indem Sie anpassen, welche Informationen zum Salesforce-Aufgabenbetrefffeld hinzugefügt werden, wenn eine Verkaufsaktivität über Sales Connect in Salesforce protokolliert wird. [Hier klicken](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) um mehr zu erfahren.

## Ankündigungen {#announcements}

* **Einstellung von Marketo Sky**: Im März wird Marketo Sky nicht mehr verfügbar sein, da wir unsere Ressourcen auf die Bereitstellung des Benutzererlebnisses der nächsten Generation konzentrieren. Im Bestreben, den Zugriff auf Funktionen aufrechtzuerhalten, die heute nur beim Marketo Sky verfügbar sind, bringen wir Asset-Ablauf und Smart Campaign Priority Override im März in das Mainstream-Erlebnis ein. [Hier klicken](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) um mehr zu erfahren.

* **Einstellung von Formularendpunkten**: Nicht unterstützte POST-Dateien für programmgesteuerte Formulare an den Endpunkt „leadCapture/save2“ werden von Marketo Engage-Formularen abgelehnt. [Hier klicken](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) um mehr zu erfahren.

**Marketo Engage-Domains - Sales-Insight-**: Bei Marketo Engage-Domains, für die kein SSL-Zertifikat bereitgestellt wurde, und https:// schlagen Aufrufe mit einem SSL-Handshake-Fehler fehl. Daher werden diese Domains eingestellt. Daher kann es vorkommen, dass Sales Insight-Benutzer mit einer älteren Konfiguration, die auf eine dieser Domains verweist, auf der Seite Lead, Kontakt, Konto, Opportunity-Panels oder Marketo Global auf Fehler bei Systembeschriftungen stoßen. Es wird empfohlen, die [Marketo Engage-Konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in Salesforce zu aktualisieren, wenn dieser Fehler auftritt. Sie müssen nur die Marketo Engage-Anmeldeinformationen aktualisieren, die im Abschnitt &quot;Marketo Sales Insight Config“ des Dokuments hervorgehoben sind.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Januar 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
