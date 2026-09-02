---
description: Der leitende Mitarbeiter von Investigate beantwortet die Fragen, die Marketing-Experten am häufigsten stellen. Es ist schneller und zuverlässiger als das manuelle Durchsuchen von Aktivitätsprotokollen, intelligentem Kampagnenverlauf und Bewertungsdatensätzen.
title: Leads untersuchen
source-git-commit: 224dff93cda319bb6bb59fcbec4edb13cc940f4a
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Leads untersuchen {#investigate-leads}

Finden Sie heraus, warum eine bestimmte Person/ein Lead einen Meilenstein (wie MQL, Programmqualifikation oder eine Kampagne) nicht erreicht hat, und erhalten Sie eine Klartext-Erklärung, was passiert ist.

>[!PREREQUISITES]
>
>Sie müssen Ansichtszugriff auf den Personen-/Lead-Datensatz und das Programm oder den Meilenstein haben, das/den Sie untersuchen.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in My Marketo auf die Kachel **Mitarbeiter für Marketo Engage**.

1. Beschreiben Sie im Eingabeaufforderungsfenster, was Sie untersuchen. Geben Sie den Lead (per E-Mail oder Name) und das an, was erwartet wurde.

   >[!NOTE]
   >
   >Beispiele: „Warum haben `john.smith@example.com` MQL im letzten Monat nicht erreicht?“ oder „Warum wurde Sato Hanako nicht zum Webinar-Programm im 3. Quartal hinzugefügt?“

1. Coworker for Marketo Engage erfasst die Aufzeichnung und den relevanten Verlauf des Leads.

1. Überprüfen Sie die Erklärung. Coworker for Marketo Engage teilt Ihnen mit, warum der Meilenstein nicht erreicht wurde und was geändert werden muss, damit der Lead sich qualifiziert.

1. basierend auf der Feststellung Maßnahmen ergreifen: ein Datenproblem korrigieren, einen Filter anpassen, den Lead-Score aktualisieren oder akzeptieren, dass das Ergebnis korrekt war.

## Anwendungsszenarien {#use-cases}

**MQL-Schwellenwert nicht erreicht**: Ein Demand Gen-Manager bemerkt einen Lead, der als interessiert gekennzeichnet wurde, aber nie MQL erreicht hat. Sie fragen: „Warum haben `david.chen@techcorp.com` MQL nicht erreicht?“ Coworker for Marketo Engage stellt fest, dass der Verhaltenswert des Leads 42 ist (8 Punkte unter dem MQL-Schwellenwert von 50) und listet die Scoring-Aktivitäten auf, die dazu beigetragen haben. Sie können genau erkennen, welche Verhaltensweisen den Lead über die Schwelle bringen würden.

**Kampagnen aufgrund von Unterdrückung überspringen**: Ein Kampagnen-Manager fragt, warum ein bestimmter Kontakt keine Einladungs-E-Mail erhalten hat, die an den Rest der Liste gesendet wurde. Der Mitarbeiter für Marketo Engage stellt fest, dass der Kontakt auf der Liste der ausgesetzten Marketing-Kontakte steht, wodurch er automatisch von allen Kampagnensendungen ausgeschlossen wird. Der Manager kontaktiert sie direkt, um herauszufinden, warum sie unterdrückt wurden.

**Fehler bei der**: Ein Marketing-Opportunity-Spezialist ist die Fehlerbehebung, warum ein Lead, der an einem Webinar teilgenommen hat, nicht in das Follow-up-Programm für die Zeit nach der Veranstaltung aufgenommen wurde. Ein Mitarbeiter von Marketo Engage verfolgt das Problem: Der Lead wurde registriert, im Veranstaltungsprogramm jedoch als „Nicht angezeigt“ gekennzeichnet, und der Folgekampagnenfilter erfordert den Status „Teilgenommen“. Der Status wurde in der Integration falsch festgelegt.

## Zu beachtende Punkte {#things-to-note}

* Lead Investigation erklärt, was basierend auf der aufgezeichneten Aktivität und Konfiguration von Marketo passiert ist. Sie kann keine Entscheidungen erklären, die außerhalb von Marketo getroffen wurden (z. B. warum ein Lead von einem Kollegen manuell entfernt wurde).
* Wenn der Aktivitätsverlauf eines Leads sehr lang ist, konzentriert sich Coworker for Marketo Engage auf die neuesten und relevantesten Ereignisse im Zusammenhang mit Ihrer Frage.
* Lead-Untersuchung ist schreibgeschützt. Sie informiert Sie zwar über die Vorfälle, ändert jedoch nichts am Lead-Datensatz oder der Programmmitgliedschaft.
* Bei Problemen, die sich als Datenqualitätsprobleme erweisen (fehlende Feldwerte, falsche Lead-Quelle), muss die Korrektur manuell im Lead-Datensatz vorgenommen werden.
* Wenn bei der Untersuchung ein Problem mit der Smart-Campaign-Logik auftritt, das sich auf viele Leads auswirkt, verwenden Sie die Programm-QA, um die vollständige Programmkonfiguration zu überprüfen.
