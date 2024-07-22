---
unique-page-id: 14352476
description: Aktivitätstyp-Feld für Aufgaben (SFDC) - Marketo-Dokumente - Produktdokumentation
title: Aktivitätstyp Feld für Aufgaben (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Aktivitätstyp Feld für Aufgaben (SFDC) {#activity-type-field-on-tasks-sfdc}

Mithilfe von Sales Connect können Sie Ihre E-Mails und Anrufe als Aktivität in Salesforce protokollieren lassen. Ein wichtiger Teil der wertvollen Daten in Salesforce besteht darin, den richtigen Wert im Feld Typ anzugeben.

>[!NOTE]
>
>Die Protokollierung von E-Mails über BCC bezieht sich nicht auf die Auswahlliste &quot;Aufgabentyp&quot;und füllt stattdessen das Feld &quot;Typ&quot;automatisch als &quot;E-Mail&quot;, da sie über Ihre BCC-Adresse an Salesforce gesendet werden.

## Anforderungen {#requirements}

* Verbindung zu Salesforce
* Kein Standardwert für Typ in der Auswahlliste &quot;Aufgabentyp&quot; ausgewählt
* Aufrufen, Antworten und E-Mail müssen alle in der Auswahlliste &quot;Aufgabentyp&quot;vorhanden sein (Großschreibung ist wichtig)
* Keine Workflows oder Trigger, die Maßnahmen zum Wert des Felds Typ ergreifen

## Setup {#setup}

Überprüfen Sie zunächst, ob die richtigen Picklist-Werte vorhanden sind. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com) und klicken Sie oben rechts auf Einrichtung .
1. Klicken Sie auf Anpassen .
1. Klicken Sie auf Aktivitäten.
1. Klicken Sie auf Aufgabenfelder .
1. Klicken Sie auf Typ.
1. Sie befinden sich jetzt in der Aufgabentyp-Auswahlliste. Stellen Sie sicher, dass kein &quot;Standard&quot;ausgewählt ist.
1. Stellen Sie sicher, dass für E-Mail, Aufruf und Antwort ein Wert vom Typ aufgeführt ist.

Nachdem dies eingerichtet ist, wird das Feld Typ den entsprechenden Wert für aufgezeichnete E-Mails, Aufrufe und Antworten anzeigen. Diese Werte werden bei Erinnerungsaufgaben in Sales Connect _nicht_ ausgefüllt.

>[!NOTE]
>
>Wenn Sie &quot;Antwort&quot;nicht als Wert sehen, fügen Sie ihn hinzu, indem Sie auf **Neu** klicken. &quot;Antwort&quot;ist kein Standardwert in Salesforce.
