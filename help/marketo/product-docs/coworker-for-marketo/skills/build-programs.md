---
description: Verwenden Sie Coworker for Marketo Engage, um ein Marketo-Programm zu erstellen, indem Sie eine vorhandene Vorlage anpassen. Holen Sie sich intelligente Kampagnen, Zeitpläne und Asset-Platzhalter, die bereit zur Überprüfung und Verfeinerung sind.
title: Erstellen von Programmen
source-git-commit: fc1bcbdaa543e39127945852a6f89e69f2966c21
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%
---
# Erstellen von Programmen {#build-programs}

Beschreiben Sie eine Marketing-Kampagne in einfacher Sprache, und Coworker for Marketo Engage passt eine vorhandene Programmvorlage an Ihre Anforderungen an, aktualisiert E-Mail-Inhalte automatisch und erstellt zusätzliche Assets, indem Sie Ihre Vorlagenstruktur duplizieren.

Die Organisationsregeln Ihres Unternehmens [, wie &#x200B;](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"} für Marketo Engage das Programm während der Erstellung strukturiert und validiert. Diese Regeln stellen sicher, dass das neue Programm mit Ihren Namenskonventionen, erforderlichen Token, Ordnerstruktur und Compliance-Standards übereinstimmt.

>[!PREREQUISITES]
>
>* Um diese Funktion nutzen zu können, müssen Sie zunächst den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
>
>* Sie müssen über die Berechtigung zum Erstellen von Programmen in Ihrem Marketo-Konto und über mindestens ein vorhandenes Marketo-Programm verfügen, das als Vorlage verwendet werden kann. Das Vorlagenprogramm sollte mindestens eine E-Mail und eine intelligente Kampagne enthalten.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in My Marketo auf die Kachel **Mitarbeiter für Marketo Engage**.

1. Ein Vorlagenprogramm auswählen. Wählen Sie ein vorhandenes Programm aus, das Ihrem Kampagnentyp entspricht (z. B. E-Mail, Webinar, Pflege).

1. Geben Sie im Eingabeaufforderungsfenster eine Beschreibung der Kampagne ein, die Sie erstellen möchten. So spezifisch oder so allgemein wie gewünscht sein (Sie können jederzeit verfeinern).

1. Coworker for Marketo Engage bestätigt seine Interpretation Ihres Briefs und listet auf, was er erstellen möchte. Überprüfen Sie dies, bevor es erstellt wird.

1. Bestätigen Sie, und Coworker for Marketo Engage erstellt das Programm in Ihrer Umgebung.

1. Öffnen Sie das neu erstellte Programm in Marketo und überprüfen Sie die Struktur.

1. Ersetzen Sie Platzhalter-E-Mail-Assets durch Ihre tatsächlichen Inhalte.

1. Überprüfen Sie, ob die Filter und Flussschritte von Smart Campaign mit Ihrer Audience und Logik übereinstimmen.

1. Führen Sie nach Abschluss aller manuellen Verfeinerungen (Konfigurieren der Smart-Campaign-Logik, Abschließen der Filter, Anpassen des E-Mail-Inhalts) [Programme validieren](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md) aus, um sicherzustellen, dass Ihre Änderungen den Organisationsregeln entsprechen, bevor Sie aktivieren.

## Anwendungsfälle {#use-cases}

**Webinar-Registrierungsprogramm**: Ein Kampagnen-Manager gibt „Erstellen Sie ein Webinar-Registrierungsprogramm für unsere August-Produktdemo. Senden Sie eine Einladungs-E-Mail, eine Erinnerung am Vortag und eine Folgenachricht mit dem Link zur Aufzeichnung danach.“ Coworker for Marketo Engage erstellt ein Programm mit drei Smart-Kampagnen (Einladung, Erinnerung, Follow-up), jeweils Platzhalter-E-Mails und einer Planung basierend auf dem Ereignisdatum.

**Trigger zur Lead-Bewertung**: Ein Marketing-Opportunity-Spezialist gibt folgende Informationen ein: „Erstellen Sie ein Programm, das Trigger erstellt, wenn ein Lead den Score 50 erreicht, und sendet sie an eine Smart List von MQL.“ Coworker for Marketo Engage erstellt das Programm mit einer Trigger-Kampagne, die auf die Score-Änderung wartet, und einem Flussschritt, der den Lead zur MQL-Liste hinzufügt.

**Erneute Interaktion fördern**: Ein Manager von Demand Gen bittet um eine 3-E-Mail-Serie zur erneuten Interaktion mit Leads, die sich seit 90 Tagen nicht mehr engagiert haben. Worker für Marketo Engage erstellt die Batch-Kampagne mit dem Inaktivitätsfilter, drei E-Mail-Sendeschritten mit entsprechenden Warteschritten zwischen ihnen und einem Flussschritt zur Aktualisierung des Lead-Status, wenn sich jemand erneut anmeldet.

**Veranstaltungsprogramm**: Nach einer Messe bittet ein Vorgesetzter einen Mitarbeiter von Marketo Engage, ein Nachbereitungsprogramm für die Veranstaltung zu erstellen, das eine Dankesnachricht an die Teilnehmer und eine E-Mail zu den verpassten Teilnehmern an die Teilnehmer sendet, die nicht angezeigt wurden. Coworker for Marketo Engage erstellt zwei Smart-Kampagnen, eine für jedes Segment, mit den richtigen Filtern und E-Mail-Platzhaltern.

>[!NOTE]
>
>In jedem obigen Beispiel klont ein Mitarbeiter eine vorhandene Programmvorlage (eine einfache E-Mail- oder Ereignisprogramm mit einer Grundstruktur) und erstellt die zusätzlichen E-Mails und Kampagnen, indem er die Vorlagen-Assets dupliziert und deren Inhalt aktualisiert. Die Flussschritte und Filter von Smart Campaign werden nach Möglichkeit angepasst. Sie müssen jedoch möglicherweise manuell verfeinert werden, um sie an die spezifische Kampagnenlogik anzupassen.

## Zu beachtende Punkte {#things-to-note}

* Klare Vorstellung davon haben, was die Kampagne tun sollte, wer die Zielgruppe ist, welche Aktion sie Trigger (oder ob es sich um einen Batch-Versand handelt) und welches Ziel sie verfolgt.
* Vorlagenauswahl ist erforderlich. Wählen Sie eine Vorlage mit mindestens einer E-Mail und einer Smart-Kampagne aus. Das Tool kann nicht mit leeren Vorlagen arbeiten.
* Der E-Mail-Inhalt wird automatisch generiert, aber die Filter und Flussschritte von Smart Campaign bleiben manuell. Sie müssen die Logik nach der Erstellung so konfigurieren, dass sie dem beabsichtigten Verhalten Ihrer Kampagne entspricht.
* Zusätzliche Assets werden durch Duplizierung erstellt. Wenn Ihre Zusammenfassung vier E-Mails erfordert, Ihre Vorlage jedoch eine enthält, erstellt das Tool drei Duplikate. Überprüfen Sie alle Elemente auf Konsistenz und übernehmen Sie das Design und die Struktur der Vorlage.
* Coworker for Marketo Engage kann nicht automatisch auf Ihre bestehenden Zielgruppenlisten zugreifen. Sie müssen die Filter der Smart-Liste manuell konfigurieren, um Ihre tatsächlichen Segmente anzusprechen, nachdem das Programm erstellt wurde.
* Komplexe mehrstufige Programme mit erweiterter Verzweigungslogik müssen nach der Erstellung möglicherweise manuell verfeinert werden.
* Wenn Ihre Marketo-Umgebung Namenskonventionen oder Ordnerstrukturen verwendet, geben Sie diese in Ihrer Zusammenfassung an, damit das Programm an der richtigen Stelle erstellt wird.
