---
description: Aktuelle Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 374f7c1bcb8c30dd914eb126c09a71c6b7ae4f90
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# Versionshinweise: Mai 2022 {#release-notes-may-22}

Unten finden Sie alle Funktionen der Version vom 22. Mai. Informieren Sie sich in Ihrer Adobe Marketo Engage Edition über die Verfügbarkeit von Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden ab der Veröffentlichung auf **6. Mai 2022**, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise eingeführt werden (sofern nicht anders angegeben).

## Native CRM-Integration {#native-crm-integration}

**Native Veeva CRM-Integration (begrenzte Verfügbarkeit)**: Verbessern Sie die Interaktion mit Fachkräften im Gesundheitswesen durch die Synchronisierung der Aktivitäten zwischen Veeva CRM und Marketo Engage über die native Integration. Diese Integration ermöglicht es Marketingexperten, für Fachkräfte im Gesundheitswesen personalisiertere und nahtlose kanalübergreifende Erlebnisse zu erstellen. Wenden Sie sich an Ihren Customer Success Manager, wenn Sie an einer Teilnahme interessiert sind.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

**Chatbot-Ereignisse für dynamischen Chat**: Verwenden Sie detailliertere Verhaltensdaten für Webbesucher, z. B. die Besuchszeit pro Seite, die Besuchszeit pro Site und den prozentualen Seitenbildlauf, um festzulegen, wann ein Chat-Dialogfeld angezeigt werden soll.

**PDF Einbetten in dynamischen Chat**: Erhöhen Sie die Interaktion und geben Sie sinnvolle Inhalte frei, indem Sie PDF in Chat-Dialogfelder einbetten und die Inhaltsleistung durch Interaktionsaktivitäten-Tracking messen.

**Erweiterte Sprachunterstützung für dynamischen Chat**: Die Benutzeroberfläche für dynamischen Chat ist jetzt auch auf Französisch, Deutsch, Japanisch, Portugiesisch und Spanisch verfügbar. Chat-Dialogfelder können auch in diesen Sprachen konfiguriert werden.

**Ausschluss von URLs für den dynamischen Chat**: Sie können steuern, auf welchen Ihrer Webseiten dynamischer Chat angezeigt wird, und bestimmte URLs von Targeting-Kriterien ausschließen.

**Verbesserungen bei der Filterung der E-Mail-Bot-Aktivität**: Schützen Sie weiterhin den Zustand Ihrer Datenbank, indem Sie neben der vorhandenen IAB-Listen-Übereinstimmungskennung auch das Bot-Verhalten anhand von versteckten Link-Benutzeragenten oder IPs und Näherungsmustern identifizieren können. Zeigen Sie Bot-Aktivitätsstatistiken an, anhand derer Sie die Anzahl der für jeden Typ identifizierten Bot-Aktivitäten nachvollziehen können.

**STS-Kopfzeile für E-Mail-Tracking-Links**: Erfüllen Sie die Best Practices für die Sicherheit mit der Möglichkeit, sichere Transport Security-Header anzuwenden, um sicherzustellen, dass Traffic zu verfolgten Links immer sicher ist.

## Erlebnis der nächsten Generation {#next-generation-experience}

**Umschalter Standardmäßig auf Erlebnis der nächsten Generation umschalten**: Der Umschalter wird in allen Bildschirmen, auf denen es verfügbar ist, standardmäßig auf das neue Erlebnis festgelegt, wodurch die Benutzer die aktualisierten Designs und Verbesserungen der Benutzerfreundlichkeit leichter erkennen können.

**Aktualisierter Bildschirm im Erlebnis der nächsten Generation**:

In der nächsten Generation liefern wir in Design Studio eine E-Mail-Vorlagendetailansicht, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bietet, auf die über den Umschalter zugegriffen werden kann.

## Erlebnisautomatisierung {#experience-automation}

**Selbstbedienungs-Flussschritte (Fortsetzung Beta)**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stapels mit der Möglichkeit, benutzerdefinierte Flussschritte zur Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Anwender als auch -Partner können diese Funktion nutzen, um die Verwendung externer Webdienste in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen (im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können).

## API-Verbesserungen {#api-enhancements}

* **Erweiterter API-Zugriff für CRM-aktivierte Abonnements**: Wir erweitern den API-Zugriff für Abonnements, für die eine CRM-Synchronisierung aktiviert ist, um Benutzern das Abrufen von Unternehmen, Chancen und Vertriebsmitarbeitern aus Marketo Engage zu ermöglichen.
* **Unterstützung für &quot;ausgeblendete&quot;Datentypen in Forms**: Bietet die Möglichkeit, ausgeblendete Formularfelder über API zu verwalten.
* **Unterstützung mehrerer Vergleichswerte für isNot Form über Regeln**: Verwalten Sie die Sichtbarkeit von Formularfeldern basierend darauf, ob der Wert eines anderen Felds nicht einer der Werte in einer bestimmten Liste ist.
* **Zulassen der Anzeige- und Sendewerte in Listen separat auswählen**: Legen Sie den Anzeigewert und den gesendeten Wert in einem Feld separat fest. Zeigen Sie beispielsweise den Namen eines Hotels an, senden Sie jedoch eine interne ID an das Backend.
* **Zulassen der Einstellung &quot;Öffnungs-Tracking deaktivieren&quot;bei &quot;E-Mail erstellen oder aktualisieren&quot;**: Erstellen Sie eine E-Mail mit deaktiviertem Öffnungs-Tracking.

## Ankündigungen {#announcements}

**E-Mail-Verifizierung und Eindeutigkeit**: Ab April wird die Einführung der E-Mail-Überprüfung beginnen. Ab diesem Zeitpunkt müssen die E-Mail-Adressen der Marketo Engage-Benutzer überprüft und eindeutig sein (dies gilt nicht für reine API-Benutzer). Für vom Verzeichnisdienst authentifizierte Benutzer werden ihre E-Mails automatisch überprüft, wenn ihr Abonnement mit E-Mail-Überprüfung aktiviert ist.

Die E-Mail-Überprüfung für Abonnements mit der Funktion &quot;Dialogfeld &quot;Anmeldung für eingeladene Benutzer&quot;oder bei denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, fällt mit der Mai-Version zusammen. Abonnements, denen eine einzelne E-Mail mit mehreren Benutzern verknüpft ist, werden mit der E-Mail-Überprüfung aktiviert und erfordern, dass diese Benutzer den Konflikt beheben und eine eindeutige E-Mail pro Benutzer verwenden. Wenn die Funktion &quot;Dialogfeld &quot;Benutzer einladen&quot;aktiviert ist, müssen über diese Funktion eingeladene Benutzer über eine eindeutige E-Mail-Adresse verfügen. Für Benutzer, die nur über diese Funktion eingeladen werden, muss die E-Mail-Adresse nicht eindeutig sein.

**Änderung des Verhaltens von Archivordnern**: Mit dieser Version ist die Möglichkeit, neue Assets in Archivordnern zu erstellen, nicht mehr in den Baumstrukturkontextmenüs verfügbar. Menüoptionen zum Erstellen neuer Assets werden für alle Assets ausgeblendet. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target=&quot;_blank&quot;}.

**_Webinar zur Produktversion_**

Nehmen Sie am 11. Mai 2022 um 9:00 Uhr PT / 23:00 Uhr ET teil, um eine [Live-Webinar](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} wird von unserem Produktteam gehostet, wo Sie erfahren können, wie Sie alle neuesten Produktinnovationen verwenden.
