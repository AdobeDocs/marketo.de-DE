---
description: Versionshinweise - Mai 2022 - Marketo-Dokumente - Produktdokumentation
title: Mai 2022 - Versionshinweise
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Mai 2022 - Versionshinweise {#release-notes-may-22}

Unten finden Sie alle Funktionen der Version vom 22. Mai. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden ab dem 6. Mai 2022 veröffentlicht. Der Rollout der verbleibenden Funktionen erfolgt schrittweise über die folgenden Wochen (sofern nicht anders angegeben).****

## Native CRM-Integration {#native-crm-integration}

**[Native VEE CRM-Integration](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (begrenzte Verfügbarkeit)**: Verbessern Sie die Interaktion mit Fachkräften im Gesundheitswesen, indem Sie die Aktivität zwischen VEE CRM und Marketo Engage über die native Integration synchronisieren. Diese Integration ermöglicht es Marketingexperten, für Fachkräfte im Gesundheitswesen personalisiertere und nahtlose kanalübergreifende Erlebnisse zu erstellen. Wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), wenn Sie an einer Teilnahme interessiert sind.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

**Chatbot-Ereignisse für Dynamic Chat**: Nutzen Sie detailliertere Verhaltensdaten für Webbesucher, z. B. die Besuchszeit pro Seite, die Besuchszeit pro Site und den Prozentsatz für den Seitenscroll, um festzulegen, wann ein Chat-Dialogfeld angezeigt werden soll.

**PDF Einbetten für Dynamic Chat**: Erhöhen Sie die Interaktion und geben Sie sinnvolle Inhalte frei, indem Sie PDF in Chatdialogfelder einbetten und die Inhaltsleistung durch Interaktionsaktivitäts-Tracking messen.

**Erweiterte Sprachunterstützung für Dynamic Chat**: Die Dynamic Chat-Benutzeroberfläche ist jetzt auch auf Französisch, Deutsch, Japanisch, Portugiesisch und Spanisch verfügbar. Chat-Dialogfelder können auch in diesen Sprachen konfiguriert werden.

**URLs für Dynamic Chat ausschließen**: Steuern Sie, auf welchen Ihrer Webseiten Dynamic Chat angezeigt wird, und schließen Sie bestimmte URLs aus den Targeting-Kriterien aus.

**[Verbesserungen bei der Filterung der E-Mail-Bot-Aktivität](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: Schützen Sie weiterhin den Zustand Ihrer Datenbank, indem Sie neben der vorhandenen IAB-Listen-Übereinstimmungsidentifizierung auch das Bot-Verhalten anhand von verborgenen Link-Benutzeragenten oder IPs und Näherungsmustern identifizieren können. Zeigen Sie Bot-Aktivitätsstatistiken an, anhand derer Sie die Anzahl der für jeden Typ identifizierten Bot-Aktivitäten verstehen können.

**[STS-Header für E-Mail-Tracking-Links](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: Erfüllen Sie die Best Practices für die Sicherheit mit der Möglichkeit, sichere Transport-Sicherheitskopfzeilen anzuwenden, um sicherzustellen, dass der Traffic zu verfolgten Links immer sicher ist.

## Erlebnis der nächsten Generation {#modern-ux}

**Umschalter Standardmäßig in Erlebnis der nächsten Generation umschalten**: Der Umschalter ist in allen Bildschirmen, auf denen er verfügbar ist, standardmäßig auf das neue Erlebnis eingestellt, wodurch Benutzer die aktualisierten Designs und Verbesserungen der Benutzerfreundlichkeit leichter erkennen können.

**Aktualisierter Bildschirm im Erlebnis der nächsten Generation**:

In der nächsten Generation stellen wir E-Mail-Vorlagendetailansicht in Design Studio bereit und bieten aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen, auf die über Umschalter zugegriffen werden kann.

## Erlebnisautomatisierung {#experience-automation}

**Schritte zum Selbstbedienungsfluss (Fortsetzung Beta)**: Erweitern Sie die Konnektivität zwischen dem Marketo Engage und dem Rest Ihres Stapels mit der Möglichkeit, benutzerdefinierte Flussschritte zur Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Anwender als auch -Partner können diese Funktion nutzen, um die Verwendung externer Webdienste in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen (im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können).

## API-Verbesserungen {#api-enhancements}

* **Erweiterter API-Zugriff für CRM-aktivierte Abonnements**: Wir erweitern den API-Zugriff für Abonnements, für die eine CRM-Synchronisierung aktiviert ist, um Benutzern das Abrufen von Unternehmen, Chancen und Vertriebsmitarbeitern von Marketo Engage zu ermöglichen.
* **Unterstützung für ausgeblendete Datentypen in Forms**: Bietet die Möglichkeit, ausgeblendete Formularfelder über API zu verwalten.
* **Mehrere Vergleichswerte für isNot Form über Regeln unterstützen**: Verwalten Sie die Sichtbarkeit von Formularfeldern basierend darauf, ob der Wert eines anderen Felds nicht einer der Werte in einer bestimmten Liste ist.
* **Einstellung &quot;Anzeige- und Sendewerte zulassen&quot;in &quot;Listen separat auswählen&quot;**: Legt den Anzeigewert und den gesendeten Wert in einem Feld separat fest. Zeigen Sie beispielsweise den Namen eines Hotels an, senden Sie jedoch eine interne ID an das Backend.
* **Allow Setting of Disable Open Tracking on Create or Update Email**: Erstellen Sie eine E-Mail mit deaktiviertem Öffnungs-Tracking.

## Ankündigungen {#announcements}

**E-Mail-Überprüfung und -Eindeutigkeit**: Ab April wird die Einführung der E-Mail-Überprüfung beginnen. Zu diesem Zeitpunkt müssen Marketo Engage-Benutzer-E-Mail-Adressen überprüft und eindeutig sein (dies gilt nicht für Nur-API-Benutzer). Für vom Verzeichnisdienst authentifizierte Benutzer werden ihre E-Mails automatisch überprüft, wenn ihr Abonnement mit E-Mail-Überprüfung aktiviert ist.

Die E-Mail-Überprüfung für Abonnements mit der Funktion &quot;Dialogfeld &quot;Anmeldung für eingeladene Benutzer&quot;oder bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, fällt mit der Mai-Version zusammen. Abonnements, denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, werden mit der E-Mail-Überprüfung aktiviert und erfordern, dass diese Benutzer den Konflikt beheben und eine eindeutige E-Mail pro Benutzer verwenden. Wenn die Funktion &quot;Dialogfeld für eingeladene Benutzer anmelden&quot;aktiviert ist, müssen über diese Funktion eingeladene Benutzer über eine eindeutige E-Mail-Adresse verfügen. Für Benutzer, die nur über diese Funktion eingeladen werden, muss die E-Mail-Adresse nicht eindeutig sein.

**Änderung des Ordnerverhaltens archivieren**: Mit dieser Version ist die Möglichkeit, neue Assets in Archivordnern zu erstellen, nicht mehr in den Baumkontextmenüs verfügbar. Menüoptionen zum Erstellen neuer Assets werden für alle Assets ausgeblendet. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar zur Produktversion_**

[Marketo Engage-Release-Webinar von März und Mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
