---
description: TBD.
title: Erstellen und Generieren von E-Mail-Kampagnen
source-git-commit: 69965ea0c32f61bf749fa6fc655854dcca7674b9
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# Erstellen und Generieren von E-Mail-Kampagnen {#build-and-generate-email-campaigns}

Erfahren Sie, wie Sie in Minuten vollständige E-Mail-Kampagnen erstellen und überprüfen können.

## Vorbereitung

Vergewissern Sie sich, dass Sie Folgendes haben:

* Ein gültiges CX Enterprise-Coworker-Konto ([hier anmelden](https://coworker-essentials.experience.adobe.com/) falls noch nicht geschehen).

* Ihre Marke wird unter **Ihre**&quot; > **Marken** eingerichtet.

* (Optional, aber empfohlen) Eine HTML-E-Mail-Vorlage, die unter **Ihr**&quot; > „E **Mail-Vorlagen“** wurde.

* Eine Zielgruppen-CSV kann hochgeladen werden.

* Eine klare Vorstellung von Ihrem Kampagnenziel (z. B. „abgelaufene Kunden zurückgewinnen“, „Benutzer zu einer Testversion einladen„).

>[!TIP]
>
>Wenn Sie mit dem Schreiben von Eingabeaufforderungen für Marketing-Kampagnen noch nicht vertraut sind, sollten Sie sich zwei Minuten Zeit nehmen, um _Prompting CX Enterprise Coworker: Best Practices_ zu überspringen.

## Schritt 1: Neuen Chat starten

Von der -Startseite aus haben Sie drei Möglichkeiten, um zu beginnen:

* Geben Sie eine Eingabeaufforderung in die zentrale Eingabeaufforderungsleiste ein.
* Wählen Sie eine vorgefertigte Kampagnenvorlage aus dem Bereich Vorlagen unter der Eingabeaufforderungsleiste.
* Verwenden Sie eine Option „help me prompt“ aus dem Dropdown-Menü in der Eingabeaufforderungsleiste, damit CX Enterprise Coworker Sie durch die Erstellung Ihrer Eingabeaufforderung führt.

[SCREENSHOT: Startseite mit hervorgehobener Eingabeaufforderungsleiste, Vorlagenzeile und hervorgehobener Option „help me prompt“]

[FOR KEITH: Kurze Beschreibung jeder Option und wann welche zu verwenden ist. Empfehlen Sie Vorlagen für Erstanbieter, Freiform-Eingabeaufforderungen für Marketing-Fachleute, die wissen, was sie möchten, und „Helfen Sie mir bei der Eingabeaufforderung“ für alle dazwischen liegenden Personen.]

## Schritt 2: Eingabeaufforderung schreiben

Eine starke CX Enterprise Coworker-Eingabeaufforderung umfasst:

* Das Kampagnenziel (was Sie erreichen möchten).
* Die Zielgruppe (für wen sie bestimmt ist oder woher die Zielgruppendaten stammen).
* Format und Struktur (Anzahl der E-Mails, Kadenz, Ton).
* Marken- oder Kontexthinweise (Verweise auf Ihre Marke, Ihr Produkt oder Ihre Kampagne).

Beispiel:

```
"Create a win-back email series for customers who bought last year but haven't returned. Use the CSV I uploaded. Include 2–3 emails that feel seasonal and remind them to shop again."
```

[FOR KEITH: Kann zwei bis drei weitere Prompt-Beispiele aus B2B und B2C hinzufügen, um Abwechslung zu schaffen. Rufen Sie aus Konsistenzgründen Anwendungsfälle aus unserem Sammlungsdokument ab.]

[SCREENSHOT: Eingabeaufforderungsleiste mit eingegebenem Beispiel-Eingabeaufforderung]

## Schritt 3: Zielgruppe hochladen

[FÜR KEITH: Anleitung zum CSV-Upload. Abdeckung: - Wo sich die Upload-Schaltfläche in der Benutzeroberfläche befindet. - Erforderliche Spalten und Formaterwartungen. - Personalisierungsfelder, die CX Enterprise-Mitarbeiter verwenden können (Vorname, Nachbestellungsdatum, Produktkategorie usw.). - Link zur Beispiel-CSV. - Was passiert, wenn Daten unübersichtlich sind oder Felder fehlen.]

[SCREENSHOT: CSV-Upload-Fluss]

>[!TIP]
>
>Schließen Sie alle Kontakte aus, die Sie nicht per E-Mail versenden möchten (abgemeldete Benutzer, interne Adressen, Testkonten), bevor Sie den Upload durchführen. Während wir die Funktion schrittweise aktivieren, um bestimmte Benutzer während der Testphase „auszuschließen“ oder „Attribute hinzuzufügen“, ist sie nicht sofort ab dem Launch-Datum verfügbar.

## Schritt 4: Kurze Beschreibung und Referenzmaterial hinzufügen

&lbrack;FÜR KEITH: Erläutern Sie, wie Sie eine Zusammenfassung, Referenzdokumente für die Marke oder einen anderen Kontext anhängen. Abdeckung: - Unterstützte Dateitypen. - Verwendung dieser Informationen durch CX Enterprise Coworker (in den Eingabeaufforderungskontext extrahiert, auf die Inhaltserstellung angewendet usw.) - Dateigrößenbeschränkungen, falls vorhanden

Hier ist ein tiefer Einblick in meine Sitzung auf dem Summit, wo ich dies hier durchgehe: https://business.adobe.com/de/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Einschränkungen - Ich kann Sie mit der Engg verbinden - Neha Pullabhotla, die uns hier bei bestimmten Themen helfen kann. &rbrack;

[SCREENSHOT: Brief-/Referenzanhang-Benutzeroberfläche]

## Schritt 5: Generieren der Kampagne

Klicken Sie **Kampagne erstellen**. CX Enterprise-Mitarbeiter:

* Erstellen Sie einen strukturierten Kampagnenplan.
* Fragen Sie nach Ihrer Zielgruppe, die auch für die Personalisierung von Inhalten verwendet wird.
* Erstellen Sie für jeden Schritt einen Entwurf für personalisierten E-Mail-Inhalt.
* Dynamisches Erstellen der Journey während des gesamten Vorgangs.
* Alles auf einem einzigen Campaign-Board zusammenstellen.

[FOR KEITH: Beschreibung des Kampagnenboards und seiner Inhalte. Bedecken Sie die Draufsicht, die Journey-Ansicht und die Inhaltsansicht. Beachten Sie, wie lange die Generierung in der Regel dauern kann - was von der Anzahl der Touchpoints auf ihrem Journey abhängt. Wenn sie einen Editor für den Workflow oder die E-Mail öffnen, wird ihnen das Gespräch angezeigt, damit sie im Kontext der spezifischen Komponente sind, wie der E-Mail-Editor ein Point-and-Click-E-Mail-Editor mit der Einschränkung ist, dass er nicht als vollständiger Designer gedacht ist, können Benutzende Bilder in Adobe Express bearbeiten oder sogar über Adobe Express eine Verbindung zu Google Drive oder AEM Assets herstellen. Alle ihre Bild-Assets werden in Express gespeichert, sie generieren Bilder in unserem E-Mail-Editor mit Firefly inline neu oder ersetzen sie durch ein lokales Bild von ihrem Computer. Sie können die HTML-Vorlage austauschen und den Inhalt neu generieren und sich schließlich eine „Test-E-Mail“ senden, um zu überprüfen, was ihr Endkunde erhalten wird]

[SCREENSHOT: Generiertes Kampagnenboard mit Plan, Journey und sichtbarem Inhalt]

## Schritt 6: Überprüfen und verfeinern

Die Gesprächsoberfläche macht die Verfeinerung einfach. Wenn Sie Änderungen vornehmen möchten, wenden Sie sich an den CX Enterprise-Mitarbeiter:

* „Machen Sie die Betreffzeile in E-Mail 2 dringender.“
* „Kürzen Sie den Textkörper für alle E-Mails.“
* „Tauschen Sie die Zielgruppe nur gegen Kunden aus der Region West aus.“
* „Fügen Sie eine vierte E-Mail mit einer stärkeren CTA hinzu.“
* „Ändern Sie die Wartezeit von 3 Tagen in 5 Tage.“

[FÜR KEITH: Hier erfahren Sie, wie Sie Änderungen sowohl im Chat als auch über die direkte Bearbeitung vornehmen können. Erläuterung der Aktualisierung von Artefakten im Kontext. Es gibt derzeit weder die Möglichkeit, dem Workflow über den Editor weitere Knoten hinzuzufügen, noch eine Versionierung. Um die bestmöglichen Ergebnisse zu erzielen, empfehlen wir ihnen auch, Änderungen für ihren gesamten Workflow ganz am Anfang der Erstellung ihres Plans anzufordern]

[SCREENSHOT: Konversationelle Verfeinerung in Aktion - Zeigt ein Vor- und Nachher einer E-Mail nach einer Chat-Anfrage an]

## Schritt 7: Durchführen eines E-Mail-Testversands

Senden Sie vor dem Start die Kampagne an sich selbst oder ein Mitglied Ihres Teams, um sie in einem echten Posteingang zu überprüfen.

[FÜR KEITH: Schritte zum Durchführen eines Testversands. Abdeckung: - Wo sich die Korrekturabzugsschaltfläche befindet. - Wer kann Testsendungen erhalten (derzeit nur der angemeldete Nutzer - ob alle E-Mails auf der Journey gesendet werden, oder nur jeweils eine (derzeit jeweils nur eine), es sei denn, der Nutzer sagt im Chat &#39;Testversand dieser Serie&#39;. - Was im Korrekturabzug zu prüfen ist (Rendering, Links, Personalisierungs-Token, Fußzeile zur Abmeldung).]

[SCREENSHOT: Testversand-Fluss]

## Schritt 8: Starten oder Exportieren

Wenn Sie mit der Kampagne zufrieden sind, haben Sie einige Optionen:

>[!NOTE]
>Launch ist derzeit nicht verfügbar, wird aber innerhalb von zwei Wochen nach der ersten Veröffentlichung aktiviert, vorbehaltlich der rechtlichen Genehmigung.

* Starten Sie die Kampagne.
* Exportieren Sie einzelne E-Mails als HTML.
* Exportieren Sie die gesamte Kampagne als Word-Dokument oder PDF zur Teamüberprüfung.

[FOR KEITH: Details zu den einzelnen Optionen und alle Prüfungen, die CX Enterprise Coworker vor der Markteinführung durchführt (Compliance, fehlerhafte Links, fehlende Personalisierungsfelder usw.).]

[SCREENSHOT: Start-/Exportoptionen]

## Häufige Fragen

&lbrack;FÜR KEITH: 4-6 FAQs basierend auf frühzeitigem Benutzerfeedback. Vorgeschlagene Einsteiger - mit unserem Eng-Team besprechen:
* „Warum dauert die erste Antwort so lange?
* „Was ist, wenn die Leistung von CX Enterprise Coworker nicht stimmt?“
* „Kann ich E-Mails direkt oder nur per Chat bearbeiten?“
* „Wie kann ich eine Kampagne speichern, ohne sie zu starten?“
* „Was passiert, wenn meine Zielgruppen-CSV Fehler aufweist?“
* „Kann ich eine Kampagne duplizieren oder neu mischen?“
* „Wie kann ich einen Kampagnenentwurf mit einem Teamkollegen zur Überprüfung freigeben?“&rbrack;
