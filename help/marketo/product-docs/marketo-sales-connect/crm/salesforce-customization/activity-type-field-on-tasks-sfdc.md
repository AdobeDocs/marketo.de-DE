---
unique-page-id: 14352476
description: Feld "Aktivität Type Field on Aufgaben (SFDC) - Marketing Docs - Produktdokumentation
title: Feld "Typ der Aktivität bei Aufgaben"(SFDC)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Feld &quot;Typ der Aktivität bei Aufgaben&quot;(SFDC) {#activity-type-field-on-tasks-sfdc}

Mithilfe von Sales Connect können Sie Ihre E-Mails und Anrufe als Aktivität in Salesforce protokollieren lassen. Ein wichtiger Aspekt für wertvolle Daten in Salesforce ist, dass das Feld Typ den richtigen Wert enthält.

>[!NOTE]
>
>Das Anmelden von E-Mails über BCC wird nicht in die Auswahlliste &quot;Aufgabe-Typ&quot;übernommen und stattdessen automatisch als &quot;E-Mail&quot;ausgefüllt, da sie über Ihre BCC-Adresse an Salesforce gesendet werden.

## Anforderungen {#requirements}

* Verbindung mit Salesforce
* In der Auswahlliste &quot;Typ der Aufgabe&quot;wurde kein Standardwert ausgewählt
* Aufruf, Antwort und E-Mail müssen alle in der Auswahlliste &quot;Aufgabe&quot;vorhanden sein (Großschreibung ist wichtig)
* Keine `Workflows` oder `Triggers` keine Aktion für den Wert des Felds &quot;Typ&quot;

## Setup {#setup}

Überprüfen Sie zunächst, ob die richtigen Werte für die Auswahlliste vorhanden sind. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

1. Navigieren Sie zu [Salesforce.com](http://Salesforce.com) und klicken Sie auf Setup in der oberen rechten Ecke.
1. Klicken Sie auf Anpassen.
1. Klicken Sie auf Aktivitäten.
1. Klicken Sie auf Aufgabe Felder.
1. Klicken Sie auf Typ.
1. Sie befinden sich jetzt in der Liste Aufgabe Type Picklist. Vergewissern Sie sich, dass kein &quot;Standard&quot;ausgewählt ist.
1. Stellen Sie sicher, dass ein Typwert für E-Mail, Aufruf und Antwort aufgeführt ist.

Sobald dies eingerichtet ist, sehen Sie, wie das Feld Typ den entsprechenden Wert für protokollierte E-Mails, Aufrufe und Antworten ausfüllt. Diese Werte werden **nicht** in Erinnerungsdaten zu Sales Connect ausgefüllt.

>[!NOTE]
>
>Wenn Sie &quot;Antworten&quot;nicht als Wert sehen, fügen Sie ihn hinzu, indem Sie auf **Neu** klicken. &#39;Antwort&#39; ist kein Standardwert in Salesforce.
