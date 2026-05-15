---
description: Verwenden Sie Marketo AI, um ein Marketo-Programm aus einer einfachen Sprachbeschreibung zu erstellen. Holen Sie sich intelligente Kampagnen, Zeitpläne und Asset-Platzhalter, die bereit zur Überprüfung und Verfeinerung sind.
title: Programm erstellen
beta: true
hide: true
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Programm erstellen {#create-program}

Beschreiben Sie eine Marketing-Kampagne im Klartext. Marketo AI erstellt die Programmstruktur mit Asset-Platzhaltern und Zeitplan.

>[!PREREQUISITES]
>
>* Um diese Funktion nutzen zu können, müssen Sie zunächst den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
>
>* Sie müssen über die Berechtigung zum Erstellen von Programmen in Ihrem Marketo-Konto verfügen.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in Ihrem Mein Marketo auf die Kachel **Mit KI erstellen**.

1. Geben Sie im Eingabeaufforderungsfenster eine Beschreibung der Kampagne ein, die Sie erstellen möchten. So spezifisch oder so allgemein wie gewünscht sein (Sie können jederzeit verfeinern).

1. Marketo AI bestätigt seine Interpretation Ihres Briefs und listet auf, was es zu erstellen beabsichtigt. Überprüfen Sie dies, bevor es erstellt wird.

1. Bestätigen Sie, und Marketo AI erstellt das Programm in Ihrer Umgebung.

1. Öffnen Sie das neu erstellte Programm in Marketo und überprüfen Sie die Struktur.

1. Ersetzen Sie Platzhalter-E-Mail-Assets durch Ihre tatsächlichen Inhalte.

1. Überprüfen Sie, ob die Filter und Flussschritte der intelligenten Kampagne mit Ihrer Audience und Logik übereinstimmen.

1. Führen Sie [Programm-QA](/help/marketo/product-docs/marketo-ai/agents/program-qa.md)-Agent vor der Aktivierung aus.

## Anwendungsszenarien {#use-cases}

**Webinar-Registrierungsprogramm**: Ein Kampagnen-Manager gibt „Erstellen Sie ein Webinar-Registrierungsprogramm für unsere August-Produktdemo. Senden Sie eine Einladungs-E-Mail, eine Erinnerung am Vortag und eine Folgenachricht mit dem Link zur Aufzeichnung danach.“ Marketo AI erstellt ein Programm mit drei Smart-Kampagnen (Einladung, Erinnerung, Follow-up), jeweils Platzhalter-E-Mails und einer Planung basierend auf dem Ereignisdatum.

**Lead-Scoring-Trigger-Kampagne**: Ein Marketing-Opportunity-Spezialist gibt den Text „Erstellen Sie ein Programm, das Trigger erzeugt, wenn ein Lead den Score 50 erreicht, und sendet sie an eine Smart List von MQL.“ ein. Marketo AI erstellt das Programm mit einer Trigger-Kampagne, die auf die Score-Änderung wartet, und einem Flussschritt, der den Lead zur MQL-Liste hinzufügt.

**Erneute Interaktion fördern**: Ein Manager von Demand Gen bittet um eine 3-E-Mail-Serie zur erneuten Interaktion mit Leads, die sich seit 90 Tagen nicht mehr engagiert haben. Marketo-KI erstellt die Batch-Kampagne mit dem Inaktivitätsfilter, drei E-Mail-Sendeschritten mit entsprechenden Warteschritten zwischen ihnen und einem Flussschritt zur Aktualisierung des Lead-Status, wenn sich jemand erneut anmeldet.

**Programm zur Veranstaltungsnachbereitung**: Nach einer Handelsmesse bittet ein Manager Marketo AI, ein Nachbereitungsprogramm für die Veranstaltung zu erstellen, das eine Dankesnachricht an die Teilnehmer und eine E-Mail zu Fehlzeiten an die Anmelder sendet, die nicht angezeigt wurden. Marketo AI erstellt zwei Smart-Kampagnen, eine für jedes Segment, mit den richtigen Filtern und E-Mail-Platzhaltern.

## Zu beachtende Punkte {#things-to-note}

* Klare Vorstellung davon haben, was die Kampagne tun sollte, wer die Zielgruppe ist, welche Aktion sie Trigger (oder ob es sich um einen Batch-Versand handelt) und welches Ziel sie verfolgt.
* Im Vorfeld sind keine Vorlagen oder Formulare erforderlich. Marketo AI erstellt die Struktur und Sie können Assets später verbinden (Sie sind weiterhin für das Schreiben von E-Mail-Kopien und das Einrichten von Landingpages verantwortlich).
* Marketo AI kann nicht automatisch auf die bestehenden Zielgruppenlisten zugreifen. Sie müssen Smart-List-Filter mit Ihren tatsächlichen Segmenten verbinden, nachdem das Programm erstellt wurde.
* Komplexe mehrstufige Programme mit erweiterter Verzweigungslogik müssen nach der Erstellung möglicherweise manuell verfeinert werden.
* Wenn Ihre Marketo-Umgebung Namenskonventionen oder Ordnerstrukturen verwendet. Geben Sie sie in Ihrer Zusammenfassung an, damit das Programm an der richtigen Stelle erstellt wird.
