---
description: Der leitende Mitarbeiter von Investigate beantwortet die Fragen, die Marketing-Experten am häufigsten stellen. Es ist schneller und zuverlässiger als das manuelle Durchsuchen von Aktivitätsprotokollen, intelligentem Kampagnenverlauf und Bewertungsdatensätzen.
title: Lead untersuchen
beta: true
hide: true
hidefromtoc: true
source-git-commit: a2c170ced2119a86ffe1f2da1bde212afa4841f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# Lead untersuchen {#investigate-lead}

Finden Sie heraus, warum eine bestimmte Person/ein Lead einen Meilenstein (wie MQL, Programmqualifikation oder eine Kampagne) nicht erreicht hat, und erhalten Sie eine Klartext-Erklärung, was passiert ist.

>[!PREREQUISITES]
>
>Sie müssen Ansichtszugriff auf den Lead-Datensatz und das Programm oder den Meilenstein haben, das/den Sie untersuchen.

## Funktionsweise

Sie teilen Marketo AI mit, welchen Lead Sie untersuchen und welche Meilensteine oder Ergebnisse Sie erwartet haben. Marketo AI untersucht den Aktivitätsverlauf des Leads, den Bewertungsdatensatz, die Programmmitgliedschaft, den Verlauf der intelligenten Kampagnenqualifizierung und alle relevanten Filter oder Unterdrückungsregeln. Anschließend wird eine klare Erklärung darüber zurückgegeben, was das erwartete Ergebnis blockiert oder verzögert hat - z. B. „Der Wert dieses Leads erreichte 48, aber der MQL-Schwellenwert ist 50“ oder „Dieser Lead wurde von der Kampagne ausgeschlossen, da er sich am 3. März abgemeldet hat.“

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in Ihrem Mein Marketo auf die Kachel **Mit KI erstellen**.

1. Beschreiben Sie im Eingabeaufforderungsfenster, was Sie untersuchen. Geben Sie den Lead (per E-Mail oder Name) und das an, was erwartet wurde.

>[!NOTE]
>
>Beispiele: „Warum haben `john.smith@example.com` MQL im letzten Monat nicht erreicht?“ oder „Warum wurde Brenda Gonzales nicht in das Webinar-Programm für das 3. Quartal aufgenommen?“

1. Marketo AI holt die Bilanz und relevante Historie des Leads auf.

1. Überprüfen Sie die Erklärung. Marketo AI gibt den spezifischen Grund an, aus dem der Milestone nicht erreicht wurde, und ggf. den Grund, der geändert werden muss, damit der Lead qualifiziert wird.

1. basierend auf der Feststellung Maßnahmen ergreifen: ein Datenproblem korrigieren, einen Filter anpassen, den Lead-Score aktualisieren oder akzeptieren, dass das Ergebnis korrekt war.

## Beispiele

**MQL-Schwellenwert nicht erreicht**
Ein Demand Gen-Manager bemerkt einen Lead, der als interessiert gekennzeichnet ist, aber nie MQL erreicht hat. Sie fragt: „Warum erreichte david.chen@techcorp.com MQL nicht?“ Marketo AI stellt fest, dass der Verhaltenswert des Leads 42 - 8 Punkte unter dem MQL-Schwellenwert von 50 - beträgt, und listet die Scoring-Aktivitäten auf, die dazu beigetragen haben. Sie kann genau erkennen, welche Verhaltensweisen den Lead über die Schwelle treiben würden.

**Kampagnenüberspringen aufgrund von Unterdrückung**
Ein Kampagnen-Manager fragt, warum eine bestimmte Kontaktperson keine Einladungs-E-Mail erhalten hat, die an den Rest ihrer Liste gesendet wurde. Marketo AI stellt fest, dass der Kontakt auf der Liste der ausgesetzten Marketing-Kontakte steht, wodurch er automatisch von allen Kampagnensendungen ausgeschlossen wird. Der Manager kontaktiert den Kontakt direkt, um zu untersuchen, warum sie unterdrückt wurden.

**Fehler bei der Programmqualifizierung**
Ein Marketing-Opportunity-Spezialist behebt Probleme, wenn ein Lead, der an einem Webinar teilgenommen hat, nicht in das Follow-up-Programm für die Zeit nach der Veranstaltung aufgenommen wurde. Die Marketo-KI verfolgt das Problem: Der Lead wurde registriert, aber im Veranstaltungsprogramm als „Nicht angezeigt“ gekennzeichnet, und der Folgekampagnenfilter erfordert den Status „Teilgenommen“. Der Status wurde in der Integration falsch festgelegt.

**Blei steckt in einer Nurture fest**
Ein Demand Gen-Manager bemerkt, dass sich ein Lead 90 Tage lang ohne Fortschritt in derselben Nurture-Phase befindet. Sie bittet Marketo AI, das zu untersuchen. Er stellt fest, dass der Interaktionswert des Leads unter den Schwellenwert gefallen ist, der erforderlich ist, um in die nächste Phase vorzustoßen, und dass der Lead seit 60 Tagen keine E-Mail geöffnet hat. Dadurch werden sie stattdessen für die Verzweigung der erneuten Interaktion qualifiziert.

## Tipps und Einschränkungen

* Die Lead-Untersuchung erklärt, was basierend auf der aufgezeichneten Aktivität und Konfiguration von Marketo passiert ist. Sie kann keine Entscheidungen außerhalb von Marketo erklären (z. B. warum ein Lead von einem Kollegen manuell entfernt wurde).
* Wenn der Aktivitätsverlauf eines Leads sehr lang ist, konzentriert sich Marketo AI auf die neuesten und relevantesten Ereignisse im Zusammenhang mit Ihrer Frage.
* Lead-Recherche ist schreibgeschützt. Sie erfahren, was passiert ist, nehmen jedoch keine Änderungen am Lead-Datensatz oder an der Programmmitgliedschaft vor.
* Bei Problemen, die sich als Datenqualitätsprobleme erweisen (fehlende Feldwerte, falsche Lead-Quelle), muss die Korrektur manuell im Lead-Datensatz vorgenommen werden.
* Wenn bei der Untersuchung ein Problem mit der Smart-Campaign-Logik auftritt, das sich auf viele Leads auswirkt, verwenden Sie die Programm-QA, um die vollständige Programmkonfiguration zu überprüfen.
