---
description: Januar 2022 - Versionshinweise zu Marketo - Produktdokumentation
title: Januar 2022 - Versionshinweise
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Versionshinweise: Januar 2022 {#release-notes-jan-22}

Die folgenden Funktionen sind in der Version vom Januar 2022 enthalten. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden ab dem 21. **2022 veröffentlicht** wobei in den folgenden Wochen für jede Funktion ein schrittweiser Rollout erfolgt (sofern nicht anders angegeben).

## Erlebnis der nächsten Generation {#modern-ux}

* **Aktualisierter Screens im Erlebnis der nächsten Generation**: Wir bieten zusätzliche, aktualisierte Bildschirme im Erlebnis der nächsten Generation, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, die über einen Umschalter zugänglich sind:

   * Asset-Details für Landingpages in [!UICONTROL Design Studio]
   * Asset-Details für Landingpages in [!UICONTROL Marketing-Aktivitäten]

## [!DNL Microsoft Dynamics]-Integration {#microsoft-dynamics-integration}

* **Synchronisierung des Feldtyps für Mehrfachauswahl-Optionssätze allgemein verfügbar**: Synchronisieren Sie den Feldtyp für Mehrfachauswahl-Optionssätze aus [!DNL Microsoft Dynamics], um ihn in Smart-Listen und Smart-Kampagnen für eine detailliertere Zielgruppenbestimmung zu nutzen. Beispiele sind: Themen/Produkte, die von Interesse sind, bevorzugte Kommunikationsformen und mehr. Diese neue Synchronisierung ist für [!DNL Microsoft Dynamics] Version 9.x verfügbar (einschließlich Dynamics 365 Online).

* **Server-zu-Server-Authentifizierung für[!DNL Microsoft Dynamics 365 Online]**: Für erhöhte Sicherheit unterstützen wir jetzt Server-zu-Server (S2S) als zusätzlichen Authentifizierungsmodus für den Marketo Engage-Synchronisierungsbenutzer in Azure Active Directory für den nicht interaktiven Zugriff auf [!DNL Microsoft Dynamics 365 Online]. Auf diese Weise können Sie die Multi-Faktor-Authentifizierung verwenden, da alle Authentifizierungen und Anmeldungen auf OAuth basieren (nur Client-ID und Client-Geheimnis).

>[!NOTE]
>
>Der S2S-Modus basiert auf dem Anwendungsbenutzer und nicht auf dem lizenzierten Benutzer, wodurch die Verwendung einer zusätzlichen Lizenz eingespart wird.

## Administration {#administration}

* **[Formularvalidierungsregeln](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Pflegen Sie den Zustand Ihrer Datenbank, indem Sie problematische oder unerwünschte E-Mail-Domains am Senden von Marketo Engage-Formularen hindern. Im Bedienfeld Globale Formularvalidierungsregel können Admins eine Blockierungsliste definieren oder eine vordefinierte Liste kostenloser Verbraucher-Domains aktivieren, die aus Formularen blockiert werden sollen.

* **[Kopfzeilensicherheit der Landingpage](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Administratoren können die Kopfzeilen „Strenge Transportsicherheit“ und „X-Frame-Optionen“ in den Domains der Landingpage verwalten, um strenge Sicherheitsanforderungen durchzusetzen.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## AEP Marketo Engage-Ziel-Connector - Erstellen neuer Leads {#aep-marketo-engage-destination-connector}

Marketo Engage-Kunden, die auch die Adobe Experience Platform (AEP) verwenden, können ihre Datenbank optimieren, indem sie neue Personendatensätze von AEP über den AEP-Ziel-Connector per Push in Marketo Engage übertragen. Beim Senden von Zielgruppensegmenten von AEP an Marketo Engage können Personen innerhalb des Segments, die noch nicht in Ihrer Marketo Engage-[ vorhanden sind, automatisch hinzugefügt ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

**[!DNL Sales Insight]für [!DNL Salesforce] CRM**

* **Neue Typ-Spalte für [!UICONTROL Beste Wetten]**: Verkäufer erhalten schnellere Einblicke mit einer neuen Spalte mit der Bezeichnung „Typ“, um auf der Seite „Beste [!UICONTROL &quot; zwischen Leads und Kontakten &#x200B;] unterscheiden.

* **[!DNL Salesforce]Platform-API-**: Als Reaktion auf [!DNL Salesforce] Einstellung der [!DNL Salesforce] Platform-API-Versionen 21.0 bis 30.0 wurde das [!DNL Sales Insight] mit den neuesten APIs aktualisiert.

* **Aktualisiertes Branding**: Alle [!DNL Sales Insight] werden aktualisiert, damit sie mit dem Adobe-Branding übereinstimmen.

**[!DNL Sales Insight]for[!DNL Microsoft Dynamics]**

* **Aktualisiertes Konto-Layout**: Verkäufer können sich einen Überblick über die wichtigsten Aktivitäten verschaffen, wie z. B. E-Mail-Aktivitäten, Web-Aktivitäten, interessante Momente und Bewertungsänderungen für alle Kontakte innerhalb eines Kontos.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Anrufergebnisse und -gründe**: Verstehen und verfolgen Sie die ausgehenden Bemühungen Ihrer Vertriebsteams detaillierter mit neuen, vollständig anpassbaren Anrufergebnis- und Anrufgrund-Optionen. Zusätzlich zu diesen neuen Feldern führen wir eine neue Governance ein, um die Auswahl der Anrufgründe und -ergebnisse zu erzwingen, während die Verkäufer Anrufe tätigen, eine neue Governance, um Anrufgründe und -ergebnisse zu aktivieren oder zu deaktivieren, und ein neues benutzerdefiniertes Feld für Anrufgrund und Anrufergebnis-[!DNL Salesforce] für die Protokollierung von Daten in [!DNL Salesforce]. [Hier klicken](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) um mehr zu erfahren.

* Anpassung der **[!DNL Salesforce]-Aktivitätsdetails**: Erfassen Sie mehr Daten zu Verkaufsaktivitäten und Aufgaben in [!DNL Salesforce], indem Sie anpassen, welche Informationen zum Betrefffeld der [!DNL Salesforce] Aufgabe hinzugefügt werden, wenn eine Verkaufsaktivität von [!DNL Sales Connect] an [!DNL Salesforce] protokolliert wird. [Hier klicken](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) um mehr zu erfahren.

## Ankündigungen {#announcements}

* **Einstellung von Marketo Sky**: Im März wird Marketo Sky nicht mehr verfügbar sein, da wir unsere Ressourcen auf die Bereitstellung des Benutzererlebnisses der nächsten Generation konzentrieren. Im Bestreben, den Zugriff auf Funktionen aufrechtzuerhalten, die heute ausschließlich Marketo Sky zur Verfügung stehen, haben wir im März Asset-Ablauf und Smart Campaign Priority Override in das Mainstream-Erlebnis integriert. [Hier klicken](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) um mehr zu erfahren.

* **Einstellung von Formularendpunkten**: Nicht unterstützte programmgesteuerte Formular-POSTs an den Endpunkt „leadCapture/save2“ werden von Marketo Engage Forms abgelehnt. [Hier klicken](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) um mehr zu erfahren.

* **Dialog „Benutzer einladen**: Im März wird die vorhandene optionale Funktion „Anmelden im Dialogfeld „Benutzer einladen“ eingestellt. Die Funktion &quot;[!UICONTROL Benutzereinladen-Dialogfeld]&quot; wird durch die Funktion „Universelle ID“ überschrieben, die für die bevorstehende Adobe Identity Management-Systemintegration erforderlich ist und im August 2021 für alle Abonnements aktiviert wurde. Aufgrund der Einstellung erzwingt Marketo Engage, dass pro E-Mail-Adresse innerhalb eines Abonnements nur ein Benutzer zugeordnet werden muss.

**Marketo Engage-Domains - [!DNL Sales Insight]-**: Bei Marketo Engage-Domains, für die kein SSL-Zertifikat bereitgestellt wurde, und https:// schlagen Aufrufe mit einem SSL-Handshake-Fehler fehl. Daher werden diese Domains eingestellt. Daher kann es vorkommen, dass [!DNL Sales Insight] Benutzer mit einer älteren Konfiguration, die auf eine dieser Domains verweist, auf ihrer Lead-, Kontakt-, Konto-, Opportunity-Bedienfelder oder Marketo Global-Seite auf Fehler bei Systembeschriftungen stoßen. Es wird empfohlen, die [Marketo Engage-](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in [!DNL Salesforce] zu aktualisieren, wenn dieser Fehler auftritt. Sie müssen nur die Marketo Engage-Anmeldeinformationen aktualisieren, die im Abschnitt &quot;[!DNL Marketo Sales Insight] Config“ des Dokuments hervorgehoben sind.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Januar 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
