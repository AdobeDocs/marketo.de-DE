---
description: Überprüfen Sie den Umfang der Daten in Marketo Engage, die Governance-Steuerelemente und die PII-Überlegungen in wichtigen Workflows wie Lead-Import, Programm-QA und Datennormalisierung.
title: Datenblatt für Mitarbeiter für Marketo Engage
source-git-commit: 224dff93cda319bb6bb59fcbec4edb13cc940f4a
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%

---

# Datenblatt für Mitarbeiter für Marketo Engage {#data-information}

Coworker for Marketo Engage ist eine native, agentische Funktion in Adobe Marketo Engage, mit der Marketing-Teams ausgewählte Workflows durch Interaktion in natürlicher Sprache automatisieren können, einschließlich Lead-Import, Programmvalidierung, Datennormalisierung, Programmerstellung, Lead-Ermittlung, Analyse und Produktanleitung. Coworker for Marketo Engage arbeitet in der bestehenden Marketo Engage-Umgebung eines Benutzers und verwendet eine von Adobe verwaltete Infrastruktur für KI-Argumentation und -Orchestrierung.

**Benutzerumgebung:** Coworker for Marketo Engage arbeitet in einer bestehenden Marketo Engage-Umgebung und führt keinen neuen Benutzer-zu-Benutzer-Freigabepfad ein.

**Datenbereich:** Der Service verarbeitet standardmäßige B2B-Marketing-Daten, die bereits in der Benutzerumgebung vorhanden sind, einschließlich Lead-Datensätzen, Programmdaten und Aktivitäten mit intelligenten Kampagnen.

**KI-Services:** Coworker for Marketo Engage nutzt einen von Adobe erstellten KI-Kabelbaum und verwendet Azure OpenAI GPT-4.1 und Claude in AWS Bedrock für KI-Argumentation, wobei Marketo MCP-Tools die Ausführung von Produktaktionen unterstützen.

**Governance:** KI-generierte Ausgaben verbleiben in der Umgebung des Benutzers und unterliegen bestehenden Governance-, Residenz- und Aufbewahrungskontrollen.

**Transparenz:** KI-generierte Ausgaben können mithilfe von Konversationen und Audit-Verlaufsdaten überprüft werden, um die Benutzeraufsicht zu unterstützen.

## Zugriffssteuerungen und Rollout

### Leads importieren

**Funktion:** Verarbeitet vom Benutzer bereitgestellte Lead-Daten für die Zuordnung, Normalisierung, Deduplizierung und den Import in Marketo Engage.

### Programme validieren

**Funktion:** Wertet Marketo-Programme anhand von Organisationsregeln aus, die von Benutzenden in einer Markdown-Datei für Kenntnisse definiert wurden, z. B. Benennungsstandards, Genehmigungsstatus, E-Mail-Compliance und Flusslogik.

<!--

### Create program from brief

**Function:** Uses natural-language prompts to generate Marketo program structures, including smart campaigns, flow steps, and content placeholders, directly within the user's environment.

### Callable agents

**Function:** Executes flow action-triggered AI actions within Smart Campaign flow steps for use cases such as validation, normalization, and bot detection.

-->

### Leads untersuchen

**Funktion:** Bietet eine konversative Analyse, warum eine Person einen Meilenstein erreicht hat oder nicht, indem die Ausführung von Flussschritten und die Mitgliedschaft in der Smart-Liste untersucht werden.

<!--

### Measurement and analytics

**Function:** Surfaces campaign and program performance analysis, including recommendations and root-cause insights.

-->

### Produktkenntnisse

**Funktion:** Bietet Best Practices und Anleitungen für Marketo über eine gemeinsame Wissensschicht, die für das gesamte Agentenerlebnis verwendet wird.

## Anwendungsszenarien

Neben den aufgeführten Programmen sollten Sie auch Coworker for Marketo Engage verwenden, um komplexe betriebliche Probleme zu diagnostizieren und zu beheben (CRM-Synchronisierungsfehler, Webhook-Fehler, Ursachenanalysen des E-Mail-Versands, Feldabweichungen), Audits in Ihrem gesamten Konto durchzuführen (E-Mail-Zustellbarkeit, Abonnement-Center-Konformität, Überprüfungen intelligenter Kampagnen, Bewertung von Modellbewertungen) und die Programmerstellung aus Briefs und Vorlagen zu beschleunigen (Veranstaltungsprogramme, mehrsprachige E-Mail-Kampagnen, Webinar-Setups). Coworker for Marketo Engage wurde entwickelt, um KI-gestützte Lead-Klassifizierung und Datenanreicherung in jedem Maßstab zu bieten, Leistungsanalysen mit Empfehlungen zur Fehlerbehebung und geführtes Debugging technischer Konfigurationen wie Velocity-Skripten und Lebenszyklusmodellen.

## Verfügbarkeit und Rollout-Status

**Berechtigung:** Bereitstellung ist auf Marketo Engage-Benutzende beschränkt, die den [Core Gen-AI-Bedingungen und den zusätzlichen Bedingungen“ zugestimmt &#x200B;](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}.

**Rollout-Modell** Die Bereitstellung von erfolgt über Alpha und Private Beta, bevor die Beta-Erweiterung für die Öffentlichkeit erweitert wird, und letztendlich allgemein verfügbar.

**Geografischer Umfang:** Die erste Version ist für Benutzende von Marketo Engage weltweit vorgesehen, mit Ausnahme von Festlandchina.

**Branchenbereich:** Der aktuelle Rollout umfasst keine vertikalen Funktionen für stark regulierte Branchen wie Gesundheitswesen, Finanzdienstleistungen, Regierung oder Verteidigung.

## Dokumentation und Support

**Dokumentation:** Die Dokumentation zu Experience League wird im Rahmen der allgemeinen Verfügbarkeit erweitert.

**Support-Modell:** Der aktuelle Support-Ansatz umfasst die Aufnahme von Benutzer-Feedback, Bürozeiten und einen Mitarbeiter für die Marketo Engage Experience League-Community.

**Service-Überwachung:** Adobe identifiziert Beobachtbarkeit, Feedback-Dashboards und Mechanismen zur Qualitätsbewertung als wichtige Komponenten für die Launch-Reife und die laufende Verbesserung.

## Daten und Ausschlüsse außerhalb des Bereichs

**Keine neuen Sonderkategoriedaten:** Coworker for Marketo Engage führt keine neue Verarbeitung von Gesundheits-, Finanz-, Standortbestimmungs-, biometrischen oder anderen Sonderkategoriedaten ein.

**Kein neuer Freigabepfad:** Der Service erstellt keinen neuen Mechanismus zum Freigeben von Inhalten zwischen Benutzenden.

**Benutzerdefinierte Ausgaben:** KI-generierte Ausgaben verbleiben unter den bestehenden Governance-Kontrollen innerhalb der bestehenden Marketo Engage-Umgebung des Benutzers.

**Aktuelle Ausschlüsse:** Der anfängliche Rollout schließt das chinesische Festland aus und bietet keine vertikalen Funktionen für stark regulierte Branchen.

## Verwendung von Azure OpenAI und Claude auf AWS Bedrock

In diesem Abschnitt wird erläutert, wie Azure OpenAI Coworker for Marketo Engage-Workflows unterstützt. Alle zugehörigen Diagramme oder Flussbeschreibungen sollten zusammen mit den hier beschriebenen Steuerelementen gelesen werden, einschließlich Einschränkungen hinsichtlich des Datenumfangs, der Benutzeraufsicht und des Modelltrainings.

**Zweck:** Azure OpenAI GPT-4.1 wird für das dialogorientierte Denken und die Orchestrierung von agentengesteuerten Workflows verwendet.

**Datenumfang:** Eingaben sind auf standardmäßige B2B-Marketing-Daten beschränkt, die bereits in der Marketo Engage-Umgebung des Benutzers vorhanden und zur Erfüllung des angeforderten Workflows erforderlich sind.

**KI-Ausgabe:** KI-Ausgaben werden durch Benutzeraufforderungen und Konfiguration bestimmt, und die Funktionen von Coworker for Marketo Engage treffen keine Entscheidungen autonom ohne Benutzerkonfiguration.

**Schulung:** Adobe verwendet keine Benutzerdaten, um Azure OpenAI-Modelle für diesen Service zu trainieren oder anzupassen.

**Benutzeraufsicht:** KI-generierte Ausgaben können innerhalb von Marketo Engage durch Konversations- und Audit-Verlaufsfunktionen überprüft werden.

## Datenaufbewahrung und -speicherung

**Benutzerdefinierte Ausgaben:** KI-generierte Ausgaben wie bereinigte Lead-Listen, QA-Berichte, generierte Programmstrukturen und normalisierte Daten verbleiben in der Marketo Engage-Umgebung des Benutzers.

**Ausrichtung der Governance** Ausgabedaten unterliegen weiterhin den in Marketo Engage bestehenden Kontrollen für Data Governance, Residence und Aufbewahrung durch den Benutzer.

**Kein neuer benutzerübergreifender Store:** Der Service führt keinen separaten Benutzer-zu-Benutzer-Datenaustauschpfad ein.

## Datenverarbeitungs- und -speicherorte

In diesem Abschnitt werden die Umgebungen zusammengefasst, in denen Coworker for Marketo Engage ausgeführt wird und wo die Verarbeitung stattfindet. Wenn das Dokument regionale Diagramme oder Infrastrukturvisualisierungen enthält, sollten diese Materialien als übergeordnete Darstellungen des Dienststandorts und des Verarbeitungsflusses und nicht als vollständige Netzwerkschemata verstanden werden.

**Anwendungsumgebung:** Coworker for Marketo Engage arbeitet in der bestehenden Adobe Marketo Engage-Umgebung des Benutzers.

**KI-Verarbeitung:** Coworker for Marketo Engage verwendet Azure OpenAI GPT-4.1 und Claude auf AWS Bedrock für konversatives Denken und Aufgabenorchestrierung.

**Speicherort der Benutzerdaten:** Benutzerdaten und KI-generierte Ausgaben verbleiben in der Marketo Engage-Umgebung des Benutzers und unterliegen den bestehenden Kontrollen für Wohnsitz, Governance und Kundenbindung des Benutzers.

**Kein separater benutzerübergreifender Speicher:** Der Service führt keine separate Benutzer-zu-Benutzer-Datenfreigabe- oder Speicherschicht ein.

## Datenbereich nach Workflow-Typ

Die von Coworker für Marketo Engage verarbeiteten Daten werden durch das Nutzungsmuster des Benutzers und den spezifischen aufgerufenen Workflow bestimmt. Nicht alle Workflows erfordern die Verarbeitung von Daten auf Lead-Ebene.

### Workflows, die nur Kampagnen-Metadaten nutzen (keine Lead-Informationen)

* Programmerstellung aus einer Zusammenfassung: Generiert Programmstrukturen, intelligente Kampagnen, Flussschritte und Platzhalter für Inhalte aus Anweisungen in natürlicher Sprache
* E-Mail-Klonen und -Übersetzung: Dupliziert und übersetzt E-Mail-Inhalte, Betreffzeilen und Marketing-Kopien in HTML-Sprachvarianten
* Kampagnenprüfung: Überprüfung der Smart-Kampagnenkonfigurationen, Trigger-/Filterdefinitionen, Flusslogik und Benennungskonventionen
* Validierung der Programm-QA: Bewertet Programme anhand benutzerdefinierter Regeln auf Kompatibilität, Genehmigungsstatus und strukturelle Vollständigkeit
* Prüfung der Abonnement-Center- und Programmarchitektur: Analysiert die Kampagnenlogik und die Programmstruktur
* Produkterkenntnisse und Best Practice-Anleitungen: Bietet Marketo Anleitungsantworten aus einer gemeinsamen Wissensschicht

### Workflows, die Datensätze auf Lead-Ebene nutzen (standardmäßige B2B-Kontaktfelder)

* Lead-Untersuchung und Fehlerbehebung: Untersucht die vom Benutzer bereitgestellten Werte der einzelnen Lead-Felder, den Aktivitätsverlauf und den Lebenszyklusverlauf, um festzustellen, warum ein Lead den MQL-Status erreicht oder nicht erreicht hat oder sich für eine Marketing-Kampagne qualifiziert hat
* Lead-Import und -Normalisierung: Verarbeitet vom Benutzer bereitgestellte Lead-Daten wie Namen, E-Mail-Adressen, Telefonnummern und Unternehmensfelder für die Zuordnung, Bereinigung und Deduplizierung
* Lead-Klassifizierung und -Anreicherung: Wertet Lead-Datensätze anhand benutzerdefinierter Scoring- oder Klassifizierungslogik aus (z. B. Gültige vs. Spam-Leads für den Zustand der Datenbank, Personalisierungspersonen, Business Leads mit Unternehmens-E-Mail-Leads vs. Verbraucher-Leads).
* Datenqualitäts- und Zustellbarkeitsprüfungen: Analysiert Interaktionsdaten auf Lead-Ebene, Bounce-Muster und doppelte Datensätze, um Probleme mit der Datenbankintegrität zu identifizieren
* Leistungsanalysen in Campaign: Oberflächen mit Lead-Interaktionsmustern, Konversionsdaten und Audience-Komposition zur Unterstützung der Leistungsanalyse

### Datenminimierung durch Design

* In allen Fällen sind die an das KI-Modell gesendeten Daten auf das beschränkt, was zur Erfüllung der spezifischen Benutzeranfrage innerhalb dieses Workflows erforderlich ist
* Coworker for Marketo Engage folgt den bestehenden Marketo Engage-Berechtigungen des Benutzers. Es bietet keinen Zugriff auf Lead-Datensätze, Felder oder Programme, über die Berechtigung des Benutzers hinaus, diese über die Produkt-Benutzeroberfläche anzuzeigen
* Benutzer, die die Lead-Daten-Verarbeitung einschränken möchten, können den Zugriff auf die Untersuchungs-Workflows des Tools durch bestehende Rollen- und Berechtigungskontrollen von Marketo Engage einschränken und gleichzeitig den vollständigen Zugriff auf strukturelle und administrative KI-Funktionen behalten

### Keine inkrementelle Datenexposition

Die KI dient als Beschleuniger für bestehende Benutzerberechtigungen und nicht als Eskalationspfad. Benutzende, die bestimmte Lead-Felder, Programme oder Partitionen in der Marketo Engage-Benutzeroberfläche nicht anzeigen können, können diese Daten auch nicht über Coworker für Marketo Engage anzeigen. Der Dienst umgeht keine Partitionsregeln, Berechtigungen auf Feldebene oder Arbeitsbereichsbeschränkungen.
