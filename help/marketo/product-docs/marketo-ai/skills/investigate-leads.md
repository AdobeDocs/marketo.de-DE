---
description: Der leitende Mitarbeiter von Investigate beantwortet die Fragen, die Marketing-Experten am häufigsten stellen. Es ist schneller und zuverlässiger als das manuelle Durchsuchen von Aktivitätsprotokollen, intelligentem Kampagnenverlauf und Bewertungsdatensätzen.
title: Leads untersuchen
badge: Beta
source-git-commit: 333381166ca4d2b89dea53c6d925e5d837d93aa6
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Leads untersuchen {#investigate-leads}

Finden Sie heraus, warum eine bestimmte Person/ein Lead einen Meilenstein (wie MQL, Programmqualifikation oder eine Kampagne) nicht erreicht hat, und erhalten Sie eine Klartext-Erklärung, was passiert ist.

>[!AVAILABILITY]
>
>Diese Funktion befindet sich derzeit in der offenen Beta-Phase. Wenden Sie sich an Ihren Account Manager, um Zugriff anzufordern. Sie müssen auch den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen.
>
>* Sie müssen Ansichtszugriff auf den Personen-/Lead-Datensatz und das Programm oder den Meilenstein haben, das/den Sie untersuchen.

>[!AVAILABILITY]
>
>Diese Funktion befindet sich derzeit in der offenen Beta-Phase. Wenden Sie sich für den Zugriff an Ihren Account Manager.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in „Meine Marketo&quot; auf die Kachel **Marketo AI** .

1. Beschreiben Sie im Eingabeaufforderungsfenster, was Sie untersuchen. Geben Sie den Lead (per E-Mail oder Name) und das an, was erwartet wurde.

   >[!NOTE]
   >
   >Beispiele: „Warum haben `john.smith@example.com` MQL im letzten Monat nicht erreicht?“ oder „Warum wurde Sato Hanako nicht zum Webinar-Programm im 3. Quartal hinzugefügt?“

1. Marketo AI holt die Bilanz und relevante Historie des Leads auf.

1. Überprüfen Sie die Erklärung. Marketo AI gibt den spezifischen Grund an, aus dem der Milestone nicht erreicht wurde, und ggf. den Grund, der geändert werden muss, damit der Lead qualifiziert wird.

1. basierend auf der Feststellung Maßnahmen ergreifen: ein Datenproblem korrigieren, einen Filter anpassen, den Lead-Score aktualisieren oder akzeptieren, dass das Ergebnis korrekt war.

## Anwendungsszenarien {#use-cases}

**MQL-Schwellenwert nicht erreicht**: Ein Demand Gen-Manager bemerkt einen Lead, der als interessiert gekennzeichnet wurde, aber nie MQL erreicht hat. Sie fragen: „Warum haben `david.chen@techcorp.com` MQL nicht erreicht?“ Marketo AI stellt fest, dass der Verhaltenswert des Leads 42 beträgt (8 Punkte unter dem MQL-Schwellenwert von 50) und listet die Scoring-Aktivitäten auf, die dazu beigetragen haben. Sie können genau erkennen, welche Verhaltensweisen den Lead über die Schwelle bringen würden.

**Kampagnen aufgrund von Unterdrückung überspringen**: Ein Kampagnen-Manager fragt, warum ein bestimmter Kontakt keine Einladungs-E-Mail erhalten hat, die an den Rest der Liste gesendet wurde. Marketo AI stellt fest, dass der Kontakt auf der Liste der ausgesetzten Marketing-Kontakte steht, wodurch er automatisch von allen Kampagnensendungen ausgeschlossen wird. Der Manager kontaktiert sie direkt, um herauszufinden, warum sie unterdrückt wurden.

**Fehler bei der**: Ein Marketing-Opportunity-Spezialist ist die Fehlerbehebung, warum ein Lead, der an einem Webinar teilgenommen hat, nicht in das Follow-up-Programm für die Zeit nach der Veranstaltung aufgenommen wurde. Die Marketo-KI verfolgt das Problem: Der Lead wurde registriert, aber im Veranstaltungsprogramm als „Nicht angezeigt“ gekennzeichnet, und der Folgekampagnenfilter erfordert den Status „Teilgenommen“. Der Status wurde in der Integration falsch festgelegt.

## Zu beachtende Punkte {#things-to-note}

* Lead Investigation erklärt, was basierend auf der aufgezeichneten Aktivität und Konfiguration von Marketo passiert ist. Sie kann keine Entscheidungen erklären, die außerhalb von Marketo getroffen wurden (z. B. warum ein Lead von einem Kollegen manuell entfernt wurde).
* Wenn der Aktivitätsverlauf eines Leads sehr lang ist, konzentriert sich Marketo AI auf die neuesten und relevantesten Ereignisse im Zusammenhang mit Ihrer Frage.
* Lead-Untersuchung ist schreibgeschützt. Sie informiert Sie zwar über die Vorfälle, ändert jedoch nichts am Lead-Datensatz oder der Programmmitgliedschaft.
* Bei Problemen, die sich als Datenqualitätsprobleme erweisen (fehlende Feldwerte, falsche Lead-Quelle), muss die Korrektur manuell im Lead-Datensatz vorgenommen werden.
* Wenn bei der Untersuchung ein Problem mit der Smart-Campaign-Logik auftritt, das sich auf viele Leads auswirkt, verwenden Sie die Programm-QA, um die vollständige Programmkonfiguration zu überprüfen.
