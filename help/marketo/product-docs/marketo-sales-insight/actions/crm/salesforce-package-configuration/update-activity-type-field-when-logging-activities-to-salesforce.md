---
description: Aktualisieren des Felds „Aktivitätstyp“ bei der Protokollierung von Aktivitäten in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Aktualisieren des Felds „Aktivitätstyp“ bei der Protokollierung von Aktivitäten in Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 6%

---

# Aktualisieren des Felds „Aktivitätstyp“ bei der Protokollierung von Aktivitäten in Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Aktionen können Ihre E-Mail- und Anrufaktivitäten automatisch mit Salesforce synchronisieren, um Berichte zu erstellen und den Aktivitätsverlauf besser sichtbar zu machen. Stellen Sie bei der Protokollierung von Aktivitäten sicher, dass das Feld Aktivitätstyp ordnungsgemäß auf E-Mail, Anruf oder Antwort aktualisiert wird, je nachdem, welcher Aktivitätstyp protokolliert wird.

>[!NOTE]
>
>Beim Protokollieren von E-Mails über BCC wird nicht die Auswahlliste „Aufgabentyp“ berücksichtigt, sondern das Feld „Typ“ automatisch als „E-Mail“ ausgefüllt, da sie über Ihre BCC-Adresse an Salesforce gesendet werden.

## Was Sie wissen sollten {#things-to-know}

* Für die Aktualisierung des Aufgabentyps ist eine Verbindung mit Salesforce erforderlich.
* In der Auswahlliste „Aufgabentyp“ sollte kein Wert „Standardtyp“ ausgewählt sein.
* Anruf, Antwort und E-Mail müssen alle in der Auswahlliste für den Aufgabentyp vorhanden sein (Groß-/Kleinschreibung wichtig).
* Workflows oder Trigger in Salesforce, die das Feld „Aufgabentyp“ aktualisieren, können diesen Prozess beeinträchtigen.

## Einrichten {#setup}

Vergewissern Sie sich zunächst, dass Sie die richtigen Werte für die Auswahlliste haben. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

Überprüfen Sie zunächst, welche Werte in Ihrer Auswahlliste für den Aufgabentyp fehlen (von E-Mail, Anruf und Antwort). Möglicherweise benötigen Sie die Hilfe Ihres Salesforce-Administrators, um dies zu überprüfen und Änderungen an Ihrer Auswahlliste für den Aktivitätstyp vorzunehmen. Um diese Änderungen vorzunehmen, kann Ihr Salesforce-Administrator die folgenden Schritte ausführen.

### In Salesforce Lightning {#salesforce-lightning}

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicken Sie auf das Zahnradsymbol in der oberen rechten Ecke und wählen Sie **Setup** > **Objekt-Manager**.
1. Geben Sie „Aufgabe“ in das Feld „Schnellsuche“ ein.
1. Klicken Sie im linken Bedienfeld auf **Felder und Beziehungen**.
1. Klicken Sie auf Feldbezeichnung **Typ**.
1. Klicken Sie unter dem Auswahllistenwert „Aufgabentyp“ auf **Neu**.
1. Geben Sie den Namen der fehlenden Auswahllistenwerte für den Aufgabentyp ein („E-Mail“, „Anruf“, „Antwort„).
1. Klicken Sie auf **Speichern**.

### In Salesforce Classic {#salesforce-classic}

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicken Sie auf **Setup** > **Erstellen** > **Anpassen** > **Aktivitäten** > **Aufgabenfelder**.
1. Klicken Sie auf **Typ**.
1. Klicken Sie unter dem Auswahllistenwert „Aufgabentyp“ auf **Neu**.
1. Geben Sie den Namen der fehlenden Auswahllistenwerte für den Aufgabentyp ein („E-Mail“, „Anruf“, „Antwort„).
1. Klicken Sie auf **Speichern**.

Nachdem dies eingerichtet ist, sehen Sie, dass das Feld Typ den entsprechenden Wert für protokollierte E-Mails, Aufrufe und Antworten ausfüllt. Diese Werte werden _nicht_ in Erinnerungsaufgaben für Sales Insight-Aktionen ausgefüllt.

>[!NOTE]
>
>Wenn Sie „Antwort“ nicht als Wert sehen, fügen Sie ihn durch Klicken auf &quot;**&quot;**. „Antwort“ ist kein Standardwert in Salesforce.

>[!MORELIKETHIS]
>
>* [Protokollieren von Attributen der Verkaufsaktivität in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Konfigurieren der Anpassung von Salesforce-Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Verkaufsaktivitäten mit Salesforce synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
