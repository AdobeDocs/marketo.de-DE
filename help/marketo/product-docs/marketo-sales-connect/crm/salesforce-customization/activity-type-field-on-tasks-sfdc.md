---
unique-page-id: 14352476
description: Aktivitätstyp-Feld für Aufgaben (SFDC) - Marketo-Dokumente - Produktdokumentation
title: Aktivitätstyp Feld für Aufgaben (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Aktivitätstyp Feld für Aufgaben (SFDC) {#activity-type-field-on-tasks-sfdc}

Mithilfe von Sales Connect können Sie Ihre E-Mails und Anrufe als Aktivität in Salesforce protokollieren lassen. Ein wichtiger Teil der wertvollen Daten in Salesforce besteht darin, den richtigen Wert im Feld Typ anzugeben.

>[!NOTE]
>
>Die Protokollierung von E-Mails über BCC bezieht sich nicht auf die Auswahlliste vom Typ Aufgabe und füllt stattdessen das Feld Typ automatisch als &quot;E-Mail&quot;, da sie über Ihre BCC-Adresse an Salesforce gesendet werden.

## Anforderungen {#requirements}

* Verbindung zu Salesforce
* Kein Standardwert für Typ in der Auswahlliste &quot;Aufgabentyp&quot; ausgewählt
* Aufrufen, Antworten und E-Mail müssen alle unter der Auswahlliste &quot;Aufgabentyp&quot;vorhanden sein (Großschreibung ist wichtig)
* Keine Workflows oder Trigger, die Maßnahmen zum Wert des Felds Typ ergreifen

## Setup {#setup}

Überprüfen Sie zunächst, ob die richtigen Picklist-Werte vorhanden sind. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com) und klicken Sie oben rechts auf Einrichtung .
1. Klicken Sie auf Anpassen .
1. Klicken Sie auf Aktivitäten.
1. Klicken Sie auf Aufgabenfelder .
1. Klick-Typ.
1. Sie befinden sich jetzt in der Liste &quot;Task Type Picklist&quot;. Stellen Sie sicher, dass kein &quot;Standard&quot;ausgewählt ist.
1. Stellen Sie sicher, dass für E-Mail, Aufruf und Antwort ein Wert vom Typ aufgeführt ist.

Nachdem dies eingerichtet ist, wird das Feld Typ den entsprechenden Wert für aufgezeichnete E-Mails, Aufrufe und Antworten anzeigen. Diese Werte werden **not** bei Erinnerungsaufgaben in Sales Connect aufgefüllt werden.

>[!NOTE]
>
>Wenn &quot;Antwort&quot;nicht als Wert angezeigt wird, fügen Sie ihn hinzu, indem Sie auf **Neu**. &quot;Antwort&quot;ist kein Standardwert in Salesforce.
