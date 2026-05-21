---
title: 2022
description: 2022 - Marketo-Dokumente - Produktdokumentation
feature: Release Information
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714id: d0251300-e25f-466f-9856-7e11ce8fa7aaid: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4d4669f3239b43afbcbd660644c8d1a35734a556
workflow-type: tm+mt
source-wordcount: 4282
ht-degree: 6%

---

# 2022

## Januar 2022 {#january}

Die folgenden Funktionen sind in der Version vom Januar 2022 enthalten. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

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

* **Neue Typ-Spalte für [!UICONTROL Beste Wetten]**: Verkäufer erhalten schnellere Einblicke mit einer neuen Spalte mit der Bezeichnung „Typ“, um auf der Seite „Beste [!UICONTROL &quot; zwischen Leads und Kontakten ] unterscheiden.

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

## März 2022 {#march}

Die folgenden Funktionen sind in der Version vom 22. März enthalten. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden ab dem 11. **2022 veröffentlicht** wobei in den folgenden Wochen für jede Funktion ein schrittweiser Rollout durchgeführt wird (sofern nicht anders angegeben).

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**: Maximieren Sie jede Gelegenheit auf Ihrer Website, indem Sie sowohl Leads als auch Konten mit proaktiven, ansprechenden und 1:1 personalisierten Konversationen ansprechen. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} ermöglicht es Marketo Engage-Benutzern, Chat als wichtigen Teil integrierter kanalübergreifender Erlebnisse für B2B-Marketing- und -Verkaufs-Anwendungsfälle zu nutzen. Zu den Funktionen gehören: die Möglichkeit, Meetings direkt im Chat zu buchen, Lead-Routing, Starter-Vorlagen, Erstellung von Konversationen per Drag-and-Drop und vieles mehr. Dynamic Chat ist in allen Marketo Engage-Paketen enthalten und wird in diesem Jahr für alle Marketo Engage-Benutzer eingeführt.

* **Verbesserung der Filterung von E-Mail** Bot-Aktivitäten: Als Erweiterung der zuvor veröffentlichten Funktion [Filterung von E-Mail-Bot-Aktivitäten](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} können Sie sich jetzt für die Protokollierung von Aktivitäten anmelden, die als Bots identifiziert werden. Anschließend können Sie Aktionen filtern und mit Triggern versehen, die auf Aktivitäten basieren, die als von Bots ausgeführt identifiziert wurden.

## Erlebnis der nächsten Generation {#modern-ux}

* **Aktualisierter Screens im Erlebnis der nächsten Generation**: Wir bieten zusätzliche, aktualisierte Bildschirme im Erlebnis der nächsten Generation, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, die über einen Umschalter zugänglich sind:

   * Formularlistenansicht in [!UICONTROL Design Studio] (einschließlich neuer Massenaktionen)

* **Programm-Workflow-Aktualisierung importieren**: Der Workflow für das Importprogramm wird in der nächsten Generation mit einem aktualisierten Design und Verbesserungen bei der Benutzerfreundlichkeit bereitgestellt. Dies ist eine automatische Änderung ohne Umschalter.

* **Admin Control für den Experience-Umschalter der nächsten Generation**: Verwalten Sie den Rollout des Erlebnisses der nächsten Generation auf eine Weise, die für Ihre Benutzer funktioniert, mit der Möglichkeit für Administratoren auszuwählen, welche Benutzertypen auf den Umschalter zugreifen können.

## Experience Automation {#experience-automation}

* **Self-Service-Flussschritte (Beta)**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Batch- und ausführbaren Kampagnen zu ermöglichen - im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können.

* **Asset-Ablauf**: Behalten Sie die Kontrolle über Ihre zeitkritischen Assets und Kampagnen bei und können Sie deren automatische Deaktivierung zu einem bestimmten Zeitpunkt im klassischen Benutzererlebnis planen.

* **Smart Campaign Priority Override**: Stellen Sie sicher, dass Smart Trigger-Kampagnen mit hoher Priorität so bald wie möglich ausgeführt werden, mit der Möglichkeit, die standardmäßige Kampagnenprioritätsrangfolge zu überschreiben. Trigger-Smart-Kampagnen mit niedrigerer Priorität können auch niedriger priorisiert werden, um Verarbeitungsressourcen für andere Aufgaben mit hoher Priorität freizugeben.

## API-Verbesserungen {#api-enhancements}

* **Zurück Öffnungsstatus von E-Mails deaktivieren**: Ermöglicht das Lesen des Öffnungsstatus von E-Mails über die API
* **Dynamische Inhaltsbetreffzeilen aus E-Mail abrufen**: Ermöglicht es Marketing-Experten, Analysen dynamischer Betreffzeilen in BI-Tools durchzuführen
* **CRUD: Benutzerdefinierte Felder für Programmteilnehmer** Ermöglicht es Marketing-Experten, benutzerdefinierte Felder für Programmteilnehmer programmgesteuert zu erstellen
* **Massenexport benutzerdefinierter Objekte aktualisiertAt-Filter**: Ermöglicht es Marketing-Experten, benutzerdefinierte Objekte programmgesteuert zu synchronisieren
* **Head Start-Einstellung für E-Mail-Programme verfügbar machen**: Ermöglicht es Marketing-Experten, E-Mail-Programme mit Head Start über die API zu konfigurieren
* **Selektive Programm-Tag-Aktualisierung**: Ermöglicht es Marketing-Experten, selektive Tag-Aktualisierungen zu übertragen, ohne alle Tags gleichzeitig zu übertragen
* **Ergebnisfeld für die Massenaktivität-Extraktion**: Ermöglicht es Marketing-Experten, zu identifizieren, welche Aktivitäten übersprungen wurden oder fehlgeschlagen sind

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## [!DNL Bizible] {#bizible}

![(Stern)](assets/yellow-star.png)

* **BI-Vorlagen**: [!DNL Bizible] bietet jetzt herunterladbare, grundlegende Reporting-Artefakte und Beispielberichte für Tableau und Power BI, um eine schnelle Entwicklung benutzerdefinierter Berichte zu ermöglichen, die auf Ihre spezifischen Geschäftsanforderungen zugeschnitten sind.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Drosselung der E-Mail-Verbindung (GA)**: Mit der Drosselung der E-Mail-Verbindung können [!DNL Sales Connect]-Admins die Versandrate von E-Mails konfigurieren, wenn Gmail oder [!DNL Exchange] als Versandkanal verwendet wird, sodass die Rate, mit der E-Mails an den Anbieter des Versandkanals übergeben werden, die erzwungenen Grenzwerte nicht überschreitet.

## Ankündigungen {#announcements}

* **Einstellung von Marketo Sky**: Im März wird Marketo Sky nicht mehr verfügbar sein, da wir unsere Ressourcen auf die Bereitstellung des Benutzererlebnisses der nächsten Generation konzentrieren. Im Bestreben, den Zugriff auf Funktionen aufrechtzuerhalten, die derzeit nur Marketo Sky zur Verfügung stehen, bringen wir Asset-Ablauf und Smart Campaign Priority Override in die klassische Version ein. [Hier klicken](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) um mehr zu erfahren.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version vom März und Mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Mai 2022 {#may}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Mai 2022 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden ab dem 6. **2022 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden (sofern nicht anders angegeben).

## Native CRM-Integration {#native-crm-integration}

**[Native Veeva CRM-Integration](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (begrenzte Verfügbarkeit)**: Verbessern Sie die Interaktion mit medizinischem Fachpersonal, indem Sie die Aktivitäten zwischen Veeva CRM und Marketo Engage über die native Integration synchronisieren. Diese Integration ermöglicht es Marketing-Experten, personalisiertere und nahtlosere Cross-Channel-Erlebnisse für medizinisches Fachpersonal zu erstellen. Wenden Sie sich an Ihren Customer Success Manager, wenn Sie an einer Teilnahme interessiert sind.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

**Chatbot-Ereignisse für[!DNL Dynamic Chat]**: Nutzen Sie detailliertere Verhaltensdaten für Web-Besucher wie die Zeit auf der Seite, die Zeit auf der Site und den Seitenscroll-Prozentsatz, um zu definieren, wann ein Chat-Dialogfeld angezeigt werden soll.

**PDF Embed for[!DNL Dynamic Chat]**: Erhöhen Sie die Interaktion und geben Sie aussagekräftige Inhalte frei, indem Sie PDFs in Chat-Dialoge einbetten und die Inhaltsleistung durch Aktivitäts-Tracking messen.

**Erweiterte Sprachunterstützung für[!DNL Dynamic Chat]**: Die [!DNL Dynamic Chat] Benutzeroberfläche ist jetzt auch auf Französisch, Deutsch, Japanisch, Portugiesisch und Spanisch verfügbar. Chatdialoge können auch in diesen Sprachen konfiguriert werden.

**URLs für[!DNL Dynamic Chat]** ausschließen: Steuern Sie, auf welcher Ihrer Web-Seiten [!DNL Dynamic Chat] angezeigt wird, und haben Sie die Möglichkeit, bestimmte URLs von den Targeting-Kriterien auszuschließen.

**[Verbesserungen bei der Filterung von E-Mail-Bot-Aktivitäten](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: Schützen Sie weiterhin die Integrität Ihrer Datenbank, indem Sie zusätzlich zur bestehenden IAB-Liste zur Identifizierung von Übereinstimmungen das Verhalten von Bots basierend auf ausgeblendeten Link-Benutzeragenten oder -IPs und Übereinstimmungsmustern identifizieren können. Zeigen Sie einen Bot-Aktivitätsstatus an, der Ihnen Aufschluss über die Anzahl der für jeden Typ identifizierten Bot-Aktivitäten gibt.

**[STS-Header für E-Mail-Tracking-Links](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: Erfüllen Sie die Best Practices für die Sicherheit mit der Möglichkeit, Secure Transport Security-Header anzuwenden, um sicherzustellen, dass der Traffic zu verfolgten Links immer sicher ist.

## Erlebnis der nächsten Generation {#modern-ux}

**Standardeinstellung für den Umschalter ist das Erlebnis der nächsten Generation**: Der Umschalter wird auf allen Bildschirmen, auf denen er verfügbar ist, standardmäßig auf das neue Erlebnis umgeschaltet, sodass Benutzende die aktualisierten Designs und Verbesserungen der Benutzerfreundlichkeit leichter entdecken können.

**Aktualisierter Bildschirm für das Erlebnis der nächsten Generation**:

Wir stellen die Detailansicht der E-Mail-Vorlage in [!UICONTROL Design Studio] im Erlebnis der nächsten Generation bereit und bieten ein aktualisiertes Design und Verbesserungen der Benutzerfreundlichkeit, auf die über den Umschalter zugegriffen werden kann.

## Experience Automation {#experience-automation}

**Self-Service-Flussschritte (weitere Betaversion)**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzende als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen (im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können).

## API-Verbesserungen {#api-enhancements}

* **Erweiterter API-Zugriff für CRM-fähige Abonnements**: Wir erweitern den API-Zugriff für Abonnements, bei denen die CRM-Synchronisierung aktiviert ist, damit Benutzende Unternehmen, Chancen und Vertriebspersonen aus Marketo Engage abrufen können.
* **Unterstützung für „ausgeblendete“ Datentypen in Forms**: Bietet die Möglichkeit, ausgeblendete Formularfelder über eine API zu verwalten.
* **Unterstützung mehrerer Vergleichswerte für isNot Form via Rules**: Verwalten der Sichtbarkeit von Formularfeldern auf der Grundlage, ob der Wert eines anderen Felds nicht einer der Werte in einer bestimmten Liste ist.
* **Zulassen, dass die Werte „Anzeige“ und „Gesendet“ in „Listen auswählen“ separat festgelegt**: Legen Sie den Anzeigewert und den gesendeten Wert in einem Feld separat fest. Beispiel: Den Namen eines Hotels anzeigen, aber eine interne ID an das Backend senden.
* **Einstellung von „Öffnungs-Tracking bei Erstellungs- oder Aktualisierungs-E-** deaktivieren“ zulassen: E-Mail mit deaktiviertem Öffnungs-Tracking erstellen.

## Ankündigungen {#announcements}

**E-Mail-Überprüfung und**: Ab April beginnt der Rollout der E-Mail-Überprüfung. Ab diesem Zeitpunkt müssen die E-Mail-Adressen der Marketo Engage-Benutzer überprüft und eindeutig sein (dies gilt nicht für Benutzer, die nur APIs nutzen). Für authentifizierte Directory Service-Benutzer werden ihre E-Mails automatisch verifiziert, wenn ihr Abonnement mit E-Mail-Verifizierung aktiviert wird.

Die E-Mail-Bestätigung für Abonnements, die die Funktion &quot;[!UICONTROL Login in Invite User Dialog] verwenden oder bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, fällt mit der Mai-Version zusammen. Abonnements, bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, werden mit der E-Mail-Überprüfung aktiviert und erfordern, dass diese Benutzer den Konflikt lösen und pro Benutzer eine eindeutige E-Mail verwenden. Wenn die Funktion „Benutzer anmelden“ im Dialogfeld „Benutzer einladen“ aktiviert ist, müssen Benutzer, die über diese Funktion eingeladen werden, über eine eindeutige E-Mail-Adresse verfügen. Für Benutzer, die nur über eine API eingeladen werden, muss die E-Mail-Adresse nicht eindeutig sein.

**Verhaltensänderung des Archivordners**: Mit dieser Version ist die Möglichkeit, neue Assets in Archivordnern zu erstellen, nicht mehr über die drei Kontextmenüs verfügbar. Menüoptionen zum Erstellen neuer Assets werden für alle Assets ausgeblendet. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version vom März und Mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Juni 2022 {#june}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Juni 2022 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

Die folgenden Funktionen werden ab dem 24. **2022 veröffentlicht** wobei die verbleibenden Funktionen in den darauffolgenden Wochen schrittweise bereitgestellt werden (sofern nicht anders angegeben).

## Marketing-Datenumgebung {#marketing-data-environment}

* **Verfügbarmachen von CreatedAt/UpdatedAt-Feldern für benutzerdefinierte Objekte**: Ermöglicht es Ihnen, diese Felder im Bildschirm „Personendetails“ zu überprüfen, um zusätzliche insight zu erhalten.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Verbesserte Benutzerfreundlichkeit von Stream Designer für[!DNL Dynamic Chat]**: Fügen Sie Karten direkt von der Arbeitsfläche von Stream Designer hinzu, ohne dass Sie sie per Drag-and-Drop verschieben müssen. Außerdem wurde die [!DNL Dynamic Chat] verbessert, um eine bessere Sichtbarkeit der Inhalte in einzelnen Karten zu ermöglichen.

* **Erweiterte Terminrouting-Regeln für[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] bietet mehr Optionen für zielgerichtetes Terminrouting. Geben Sie an, welche Agententermine auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, um sicherzustellen, dass Leads an die entsprechenden Agenten weitergeleitet werden.

* **Erweiterte Dialogfeldberichte für[!DNL Dynamic Chat]**: Sehen Sie sich die Leistung Ihrer [!DNL Dynamic Chat] Kampagnen genauer an, indem Sie völlig neue Datenvisualisierungen für Interaktions- und Konversionsmetriken verwenden.

* **Nicht verwendete Marketo Engage-Attribute für[!DNL Dynamic Chat]** synchronisieren: Heben Sie die Synchronisierung von nicht verwendeten Marketo Engage-Attributen mit Ihrem [!DNL Dynamic Chat] auf, um die Datenbereinigung zu erleichtern und alternative Attribute nach Bedarf zu synchronisieren.

## Erlebnis der nächsten Generation

**Neue Umschaltansichten ein/aus**: Die folgenden Ansichten sind jetzt in der nächsten Generation verfügbar:

* [E-Mail-Detailansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [E-Mail-Listenansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Experience Automation {#experience-automation}

* **Ausschlüsse für globale Formularfeldvalidierungsregeln**: Schließen Sie bestimmte Formulare von globalen Formularvalidierungsregeln aus, damit Abonnementzentren und andere geschäftskritische Workflows alle Werte akzeptieren können.

* **Self-Service-Flussschritte**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen. Im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können.

* **Munchkin Protocol Agnostic Link Tracking**: Erweitern Sie die Unterstützung für das Tracking von `tel`- und `mailto`-Links mit Munchkin, um erweiterte Webverhaltensweisen zu verfolgen.

* **Zusätzliche HTTP-Methoden für Webhooks**: Geben Sie PUT, PATCH und DELETE als Anfragetypen für die Interaktion mit Webservices an.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[!DNL Sales Insight]Berechtigungssatz in[!DNL Salesforce]**: Administratoren können über den Berechtigungssatz für Marketo-Apps, der Teil des [!DNL Sales Insight]-[!DNL Salesforce] ist, [!DNL Sales Insight] Zugriff für eine begrenzte Anzahl von Personen auf Benutzerebene statt auf Profilebene gewähren.

* **Mein Marketo-Kachel-Update - [!DNL Sales Insight] Aktionen**: Marketo-Administratoren (und von ihnen benannte Benutzer) können jetzt über eine neue Kachel [!DNL Sales Insight] Aktionen auf der Seite Mein Marketo schnell zu ihrer [!DNL Sales Insight]-Instanz navigieren.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **[!DNL Salesforce]API-Update**: Mit der [!DNL Salesforce] Summer &#39;22-Version werden die API-Legacy-Versionen 21 bis 30 von [!DNL Salesforce] nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle [!DNL Sales Connect], die ältere API-Versionen verwenden, so aktualisiert, dass sie innerhalb einer unterstützten Version bleiben. Ausführliche Informationen zu [!DNL Salesforce] API-Pensionsplänen finden Sie [hier](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die API zum Extrahieren von Massenprogrammmitgliedern**: Filtern nach Programmmitgliedschaftsstatus, updatedAt, Kadenz oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der API für die Massenprogrammextraktion**: Geben Sie während der Auftragserstellung bis zu 10 Programme an, um den Durchsatz zu verbessern.

## Ankündigungen {#announcements}

* **Einstellung von Forms - Forms 1.0, Lead-Erfassungs-/Speicherendpunkt und No-Script-Versionen von Forms**: Die Unterstützung für Forms 1.0-Assets wird bis Oktober 2022 vollständig aus Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Marketo Engage-Formulare erfordern, dass JavaScript auf Landingpages und Websites geladen wird.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## August 2022 {#august}

Unten finden Sie alle Funktionen, die in der Version vom 22. August enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

Mit den folgenden Funktionen wurde am 26. **2022 ein schrittweiser Rollout**.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* Alle veröffentlichten Dialogfelder gleichzeitig aktivieren/deaktivieren für [!DNL Dynamic Chat]**: Alle veröffentlichten Dialogfelder gleichzeitig global aktivieren/deaktivieren auf der Konfigurationsseite mit einem Klick.

* **Benutzerdefinierte Avatare für[!DNL Dynamic Chat]**: Laden Sie einen benutzerdefinierten Chatbot-Avatar hoch, damit er für Ihre Marke personalisiert werden kann.

* **Chat-Transkripte für[!DNL Dynamic Chat]**: Zeigen Sie Chat-Transkripte für jede Konversation an, um tiefere Informationen darüber zu erhalten, was jeden Web-Besucher interessiert.

## Erlebnis der nächsten Generation

* **Adobe-Branding**: Aktualisiertes Erscheinungsbild für Editoren und Personendetailseiten mit neuem Adobe Experience Cloud-Branding.

* **Ordnerhierarchie des Zielordners im Dialogfeld „Verschieben“ anzeigen**: Die Anzeige der Ordnerhierarchie für jeden Ordner erleichtert das Verschieben von Assets und verringert die Wahrscheinlichkeit, dass sie sich in einem falschen Ordner befinden.

* **[Aktualisierter Screens im Erlebnis der nächsten Generation](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**: Wir bieten zusätzliche, aktualisierte Bildschirme im Erlebnis der nächsten Generation, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, die über einen Umschalter zugänglich sind:

   * Snippet-Details
   * Details zu „Bildern und Dateien“

>[!NOTE]
>
>Die Ausnahme besteht darin, ein Asset in einen Ordner innerhalb eines Programms in Marketing-Aktivitäten zu verschieben. Bei dieser Aktion zum Verschieben wird die Ordnerhierarchie nicht angezeigt, da Ordner innerhalb eines Programms keine doppelten Namen haben können.

## Experience Automation {#experience-automation}

* **[Self-Service-Flussschritte - Verbesserungen beim Programmimport](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**: Verbesserte Unterstützung für den Import von Programmen mit benutzerdefinierten Flussschritten, wobei Sie jetzt mehrere Instanzen desselben Dienstleisters verwenden und Programme importieren können, die mit diesen Dienstleistern kompatible Flussschritte aufweisen.

* **[!DNL Munchkin]- Erweiterte Link-Überwachung**: Erweitern der Unterstützung für die Verfolgung von `tel` und `mailto` Links mit Munchkin, um eine erweiterte Reihe von Web-Verhaltensweisen zu verfolgen.

* **Sichtbarkeit der benutzerdefinierten Webhook-Kopfzeile**: Die benutzerdefinierten Webhook-Kopfzeilen werden jetzt auf der Registerkarte [!UICONTROL Admin] > [!UICONTROL Webhooks] angezeigt, um die Sichtbarkeit zu verbessern.

* **CAPTCHA**: Auswerten der Gültigkeit von Formularübermittlungen [mithilfe von reCAPTCHA v3](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} zur Bewertung des eingehenden Formular-Traffics. Erstellen Sie Marketing-Workflows, um verdächtigen Bot-Traffic automatisch auszuschließen, unter Quarantäne zu stellen oder zu löschen.

* **Berechtigung zum Genehmigen eines Formulars**: Neue Berechtigung zum Steuern, welche Designer Änderungen an einem Formular in Übereinstimmung mit anderen [!UICONTROL Design Studio]-Assets genehmigen können. Dadurch wird verhindert, dass andere Designer Änderungen an Formulare pushen, ohne dass eine andere Person mit der Berechtigung Genehmigung diese überprüft.

* **Kampagnenwiederholung nach anonymer Zusammenführung immer durchführen**: Die anonyme Lead-Zusammenführung erfolgt vor der Kampagnenwiederholung, sodass sich benutzerdefinierte Feldfilter zuverlässig verhalten, wenn die anonyme Kampagnenwiederholung durchgeführt wird.

## Marketing-Datenumgebung {#marketing-data-environment}

* **Kürzung der Benutzeroberfläche von Feldern des benutzerdefinierten Objekts &quot;[!UICONTROL Verwendet von]&quot;**: Es ist jetzt einfacher, benutzerdefinierte Objektfelder zu identifizieren, die „in Verwendung“ sind, sodass Sie bei Bedarf Felder aus einem benutzerdefinierten Objekt löschen können.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die API zum Extrahieren von Massenprogrammmitgliedern**: Filtern nach Programmmitgliedschaftsstatus, updatedAt, Kadenz oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Integration mit [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**: Zeigen Sie Aktivitäten aus [!DNL Dynamic Chat] im [!DNL Sales Insight] Panel an und nutzen Sie diesen neuen Datenpunkt bei der Kundenakquise.

## Ankündigungen {#announcements}

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Oktober 2022 {#october}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Oktober 2022 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **Samstag, 14. Oktober 2022** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie im Folgenden jede Funktion auf ihren Status.

### Marketing-Datenumgebung {#marketing-data-environment}

</br>

* **Benutzerdefinierte Feldsynchronisierung für Programmteilnehmer**: Möglichkeit zur bidirektionalen Synchronisierung erweiterbarer Felder, die für ein Programmmitglied erfasst wurden (z. B. Teilnehmervoreinstellungen bei der Ereignisregistrierung wie Essen, Sitzungen, Tracks usw.) mit den Feldern für Kampagnenmitglieder in Salesforce.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Synchronisieren benutzerdefinierter Felder für Programmmitglieder</a></td>
  </tr>
  </tbody>
</table>

* **Adobe Privacy Service-Integration**: Harmonisieren Sie sich mit Privacy Service, um die Einhaltung von Datenschutzbestimmungen bei allen Experience Cloud-Produkten zu automatisieren. Derzeit ist dieser Service nur für Marketo Engage-Kunden verfügbar, die sich für das Adobe Identity Management-System entschieden haben.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Erlebnis der nächsten Generation {#modern-ux}

</br>

* **Aktualisierter Screens im Erlebnis der nächsten Generation**: Wir bieten zusätzliche, aktualisierte Bildschirme im Erlebnis der nächsten Generation, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, die über einen Umschalter zugänglich sind:

   * Details zu Landingpage-Vorlagen
   * E-Mail-Vorlagenliste

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Umschalter</a></td>
  </tr>
  </tbody>
</table>

* **Registerkarte Verwendet von in E-Mail-Vorlagendetails**: In der neuen -Version werden zusätzliche Informationen zu Assets angezeigt, die die E-Mail-Vorlage verwenden, darunter Asset-Status, Zuletzt geändert und Zuletzt geändert von. Sie können die Liste der von Assets verwendeten Assets auch durchsuchen, sortieren und filtern.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

* **Bericht-Asset-Filter-Modale**: Neuer Entwurf für Berichtskonfigurations-Modale mit einer neuen Asset-Baumstruktur im Konfigurationsmenü und einem Filter für das Erstellungsdatum und das Änderungsdatum.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

### API-Verbesserungen {#api-enhancements}

</br>

* **Massenimport von Leads: Vertriebsmitarbeiterzuordnung**: Parität mit der Lead-REST-API, um Leads während des Massenimportvorgangs von Leads mit Vertriebsmitarbeitern verknüpfen zu können, was die Komplexität und die Anzahl der erforderlichen API-Aufrufe reduziert.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Massenimport von Leads</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(Stern)](assets/yellow-star.png)

* **Integration von Sales Insight mit Dynamic Chat**: Das Insights-Dashboard enthält jetzt Dynamic Chat-Aktivitäten im Smart Grid sowie eine wöchentliche Zusammenfassung und Detailkarten.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integration von Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Funktionen für Agile Versionen

Die folgenden Funktionen folgen einem Agile-Format und werden an verschiedenen Daten vor oder nach dem standardmäßigen Veröffentlichungsdatum veröffentlicht. Bitte überprüfen Sie im Folgenden jede Funktion auf ihren Status.

* **Dialog-Streams automatisch anordnen für Dynamic Chat**: Verbessern Sie Ihre überfüllte Dialog-Arbeitsfläche, indem Sie alles auf der Arbeitsfläche in einem sauberen und leicht lesbaren Format organisieren.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Designer-Symbole streamen</a></td>
  </tr>
  </tbody>
</table>

* **Meeting-Links für Dynamic Chat**: Option zum automatischen Einfügen eines Teams- oder Meet-Links für Google und Outlook in jede Kalendereinladung, die an Besuchende gesendet wird.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Kalender</a></td>
  </tr>
  </tbody>
</table>

* **Unterstützung zusätzlicher Datentypen für Dynamic Chat**: Drei neue Datentypen (boolesch, Ganzzahl, Gleitkommazahl) ermöglichen es Ihnen, mehr bestehende Marketo Engage-Felder in Dynamic Chat für Dinge wie das Targeting anhand von Scores oder das Stellen von Ja-/Nein-Fragen an Besuchende zu nutzen.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Dokumentation – Aktualisierungen</b></td>
  </tr>
  <tr>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

## Ankündigungen {#announcements}

* **Forms 1.0**: Die Einstellung von Forms 1.0 wird mit der Oktober-Version abgeschlossen. Forms 1.0-Assets können keine Daten mehr an Marketo Engage senden und geben Fehler zurück, wenn versucht wird.

* **No-Script Forms**: Forms funktioniert nicht mehr, wenn JavaScript im Browser deaktiviert ist. Für die Formularübermittlung muss JavaScript aktiviert sein.
