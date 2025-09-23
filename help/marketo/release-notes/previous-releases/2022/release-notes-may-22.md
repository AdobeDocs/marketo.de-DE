---
description: Mai 2022 - Versionshinweise zu Marketo - Produktdokumentation
title: Mai 2022 – Versionshinweise
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 4%

---

# Versionshinweise – Mai 2022 {#release-notes-may-22}

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

## Erlebnis der nächsten Generation {#modern-ux}

**Standardeinstellung für den Umschalter ist das Erlebnis der nächsten Generation**: Der Umschalter wird auf allen Bildschirmen, auf denen er verfügbar ist, standardmäßig auf das neue Erlebnis umgeschaltet, sodass Benutzende die aktualisierten Designs und Verbesserungen der Benutzerfreundlichkeit leichter entdecken können.

**Aktualisierter Bildschirm für das Erlebnis der nächsten Generation**:

Wir stellen die Detailansicht der E-Mail-Vorlage in [!UICONTROL Design Studio] im Erlebnis der nächsten Generation bereit und bieten ein aktualisiertes Design und Verbesserungen der Benutzerfreundlichkeit, auf die über den Umschalter zugegriffen werden kann.

## Experience Automation {#experience-automation}

**Self-Service-Flussschritte (weitere Betaversion)**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzende als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen (im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können).

## API-Verbesserungen {#api-enhancements}

* **Erweiterter API-Zugriff für CRM-fähige Abonnements**: Wir erweitern den API-Zugriff für Abonnements, bei denen die CRM-Synchronisierung aktiviert ist, damit Benutzende Unternehmen, Chancen und Vertriebspersonen aus Marketo Engage abrufen können.
* **Unterstützung für „ausgeblendete“ Datentypen in Forms**: Bietet die Möglichkeit, ausgeblendete Formularfelder über eine API zu verwalten.
* **Unterstützung mehrerer Vergleichswerte für isNot Form via Rules**: Verwalten der Sichtbarkeit von Formularfeldern auf der Grundlage, ob der Wert eines anderen Felds nicht einer der Werte in einer bestimmten Liste ist.
* **Zulassen, dass die Werte „Anzeige“ und „Gesendet“ in „Listen auswählen“ separat festgelegt**: Legen Sie den Anzeigewert und den gesendeten Wert in einem Feld separat fest. Beispiel: Den Namen eines Hotels anzeigen, aber eine interne ID an das Backend senden.
* **Einstellung von „Öffnungs-Tracking bei Erstellungs- oder Aktualisierungs-E-** deaktivieren“ zulassen: E-Mail mit deaktiviertem Öffnungs-Tracking erstellen.

## Ankündigungen {#announcements}

**E-Mail-Überprüfung und**: Ab April beginnt der Rollout der E-Mail-Überprüfung. Ab diesem Zeitpunkt müssen die E-Mail-Adressen der Marketo Engage-Benutzer überprüft und eindeutig sein (dies gilt nicht für Benutzer, die nur APIs nutzen). Für authentifizierte Directory Service-Benutzer werden ihre E-Mails automatisch verifiziert, wenn ihr Abonnement mit E-Mail-Verifizierung aktiviert wird.

Die E-Mail-Bestätigung für Abonnements, die die Funktion &quot;[!UICONTROL Login in Invite User Dialog] verwenden oder bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, fällt mit der Mai-Version zusammen. Abonnements, bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, werden mit der E-Mail-Überprüfung aktiviert und erfordern, dass diese Benutzer den Konflikt lösen und pro Benutzer eine eindeutige E-Mail verwenden. Wenn die Funktion „Anmelden im Dialogfeld Benutzer einladen“ aktiviert ist, müssen Benutzer, die über diese Funktion eingeladen werden, über eine eindeutige E-Mail-Adresse verfügen. Für Benutzer, die nur über eine API eingeladen werden, muss die E-Mail-Adresse nicht eindeutig sein.

**Verhaltensänderung des Archivordners**: Mit dieser Version ist die Möglichkeit, neue Assets in Archivordnern zu erstellen, nicht mehr über die drei Kontextmenüs verfügbar. Menüoptionen zum Erstellen neuer Assets werden für alle Assets ausgeblendet. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version vom März und Mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
