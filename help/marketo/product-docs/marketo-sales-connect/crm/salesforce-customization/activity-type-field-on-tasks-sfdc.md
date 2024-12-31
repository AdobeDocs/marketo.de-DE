---
unique-page-id: 14352476
description: 'Aktivitätstyp: Feld „Aufgaben“ (SFDC) - Marketo-Dokumente - Produktdokumentation'
title: Feld „Aktivitätstyp“ für Aufgaben (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Feld „Aktivitätstyp“ für Aufgaben (SFDC) {#activity-type-field-on-tasks-sfdc}

Mithilfe von Sales Connect können Sie Ihre E-Mails und Anrufe als Aktivität in Salesforce protokollieren lassen. Eine wichtige Voraussetzung für wertvolle Daten in Salesforce ist, dass das Feld Typ den richtigen Wert eingibt.

>[!NOTE]
>
>Die Protokollierung von E-Mails über BCC erfolgt nicht über die Auswahlliste „Aufgabentyp“, sondern es wird stattdessen automatisch „E-Mail“ im Feld „Typ“ angezeigt, da die E-Mails über Ihre BCC-Adresse an Salesforce gesendet werden.

## Anforderungen {#requirements}

* Verbindung mit Salesforce
* Kein Standardtypwert in der Auswahlliste „Aufgabentyp“ ausgewählt
* Anruf, Antwort und E-Mail müssen alle unter der Auswahlliste „Aufgabentyp“ vorhanden sein (Groß-/Kleinschreibung wichtig)
* Keine Workflows oder Trigger, die Aktionen mit dem Wert des Felds Typ durchführen

## Einrichten {#setup}

Vergewissern Sie sich zunächst, dass Sie die richtigen Werte für die Auswahlliste haben. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com) und klicken Sie oben rechts auf Setup .
1. Klicken Sie auf Anpassen.
1. Klicken Sie auf Aktivitäten.
1. Klicken Sie auf Aufgabenfelder.
1. Klicken Sie auf Typ.
1. Sie befinden sich jetzt in der Auswahlliste „Aufgabentyp“. Stellen Sie sicher, dass keine „Standard“ ausgewählt ist.
1. Stellen Sie sicher, dass für E-Mail, Anruf und Antwort ein Wert vom Typ aufgeführt ist.

Nachdem dies eingerichtet ist, sehen Sie, dass das Feld Typ den entsprechenden Wert für protokollierte E-Mails, Aufrufe und Antworten ausfüllt. Diese Werte werden _nicht_ in Sales Connect-Erinnerungsaufgaben ausgefüllt.

>[!NOTE]
>
>Wenn Sie „Antwort“ nicht als Wert sehen, fügen Sie ihn durch Klicken auf &quot;**&quot;**. „Antwort“ ist kein Standardwert in Salesforce.
