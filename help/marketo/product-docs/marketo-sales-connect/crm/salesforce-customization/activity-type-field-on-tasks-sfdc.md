---
unique-page-id: 14352476
description: 'Aktivitätstyp: Feld „Aufgaben“ (SFDC) - Marketo-Dokumente - Produktdokumentation'
title: Feld „Aktivitätstyp“ für Aufgaben (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# Feld „Aktivitätstyp“ für Aufgaben (SFDC) {#activity-type-field-on-tasks-sfdc}

Mithilfe von [!DNL Sales Connect] können Sie Ihre E-Mails und Anrufe als Aktivität in [!DNL Salesforce] protokollieren lassen. Eine wichtige Voraussetzung für wertvolle Daten in [!DNL Salesforce] ist, dass das Feld [!UICONTROL Typ] den richtigen Wert ausfüllt.

>[!NOTE]
>
>Die Protokollierung von E-Mails über BCC erfolgt nicht auf der Auswahlliste „Aufgabentyp“, sondern es wird stattdessen automatisch „E-Mail“ im Feld „Typ“ angezeigt, da die E-Mails über Ihre BCC-Adresse an [!DNL Salesforce] gesendet werden.

## Anforderungen {#requirements}

* Verbindung mit [!DNL Salesforce]
* Kein Standardtypwert in der Auswahlliste „Aufgabentyp“ ausgewählt
* Anruf, Antwort und E-Mail müssen alle unter der Auswahlliste „Aufgabentyp“ vorhanden sein (Groß-/Kleinschreibung wichtig)
* Keine Workflows oder Trigger, die Aktionen mit dem Wert des Felds Typ durchführen

## Einrichten {#setup}

Vergewissern Sie sich zunächst, dass Sie die richtigen Werte für die Auswahlliste haben. Sie benötigen die Hilfe Ihres [!DNL Salesforce], um Änderungen an Ihrer Auswahlliste vorzunehmen.

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com) und klicken Sie oben rechts auf Setup .
1. Klicken Sie auf **[!UICONTROL Anpassen]**.
1. Klicken Sie auf **[!UICONTROL Aktivitäten]**.
1. Klicken Sie **[!UICONTROL Aufgabenfelder]**.
1. Klicken Sie auf **[!UICONTROL Typ]**.
1. Sie befinden sich jetzt in der Auswahlliste „Aufgabentyp“. Stellen Sie sicher, dass keine „Standard“ ausgewählt ist.
1. Stellen Sie sicher, dass ein [!UICONTROL Type]-Wert für [!UICONTROL Email], [!UICONTROL Call] und [!UICONTROL Reply] aufgeführt ist.

Nachdem dies eingerichtet ist, sehen Sie, dass das Feld Typ den entsprechenden Wert für protokollierte E-Mails, Aufrufe und Antworten ausfüllt. Diese Werte werden _nicht_ in Sales Connect-Erinnerungsaufgaben ausgefüllt.

>[!NOTE]
>
>Wenn Sie „Antwort“ nicht als Wert sehen, fügen Sie ihn durch Klicken auf &quot;**[!UICONTROL &quot;]**. „Antwort“ ist in [!DNL Salesforce] kein Standardwert.
