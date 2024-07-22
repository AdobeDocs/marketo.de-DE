---
description: Feld "Aktivitätstyp aktualisieren"bei der Protokollierung von Aktivitäten in Salesforce - Marketo Docs - Produktdokumentation
title: Feld "Aktivitätstyp"bei der Protokollierung von Aktivitäten in Salesforce aktualisieren
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 1%

---

# Feld &quot;Aktivitätstyp&quot;bei der Protokollierung von Aktivitäten in Salesforce aktualisieren {#update-activity-type-field-when-logging-activities-to-salesforce}

Mit Aktionen können Sie Ihre E-Mail- und Aufrufaktivitäten automatisch mit Salesforce synchronisieren, um sie für die Berichterstellung zu verwenden, und die Sichtbarkeit des Aktivitätsverlaufs erhöhen. Stellen Sie bei der Protokollierung von Aktivitäten sicher, dass das Feld Aktivitätstyp entsprechend dem protokollierten Aktivitätstyp ordnungsgemäß in E-Mail, Aufruf oder Antwort aktualisiert wird.

>[!NOTE]
>
>Die Protokollierung von E-Mails über BCC bezieht sich nicht auf die Auswahlliste &quot;Aufgabentyp&quot;und füllt stattdessen das Feld &quot;Typ&quot;automatisch als &quot;E-Mail&quot;, da sie über Ihre BCC-Adresse an Salesforce gesendet werden.

## Was zu wissen ist {#things-to-know}

* Eine Verbindung mit Salesforce ist erforderlich, damit der Aufgabentyp aktualisiert werden kann.
* In der Auswahlliste &quot;Aufgabentyp&quot;sollte kein Standardwert vom Typ ausgewählt sein.
* Aufrufen, Antworten und E-Mail müssen alle in der Auswahlliste &quot;Aufgabentyp&quot;vorhanden sein (Großschreibung ist wichtig).
* Workflows oder Trigger in Salesforce, die das Feld &quot;Task Type&quot;aktualisieren, können diesen Vorgang beeinträchtigen.

## Setup {#setup}

Überprüfen Sie zunächst, ob die richtigen Picklist-Werte vorhanden sind. Sie benötigen die Hilfe Ihres Salesforce-Administrators, um Änderungen an Ihrer Auswahlliste vorzunehmen.

Überprüfen Sie zunächst, welche Werte in Ihrer Aufgabentyp-Auswahlliste fehlen (aus E-Mail, Aufruf und Antwort). Möglicherweise benötigen Sie die Hilfe Ihres Salesforce-Administrators, um dies zu überprüfen und Änderungen an Ihrer Auswahlliste für Aktivitätstypen vorzunehmen. Um diese Änderungen vorzunehmen, kann Ihr Salesforce-Administrator die folgenden Schritte ausführen.

### In Salesforce Lightning {#salesforce-lightning}

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einrichtung** > **Objektmanager** aus.
1. Geben Sie &quot;task&quot;in das Feld &quot;Schnellsuche&quot;ein.
1. Klicken Sie im linken Bereich auf **Felder und Beziehungen**.
1. Klicken Sie auf die Feldbezeichnung **Typ**.
1. Klicken Sie unter &quot;Task Type Picklist Value&quot;auf **New**.
1. Geben Sie den Namen der fehlenden Task Type Picklist-Werte ein (&quot;E-Mail, &quot;Aufruf&quot;, &quot;Antwort&quot;).
1. Klicken Sie auf **Speichern**.

### In Salesforce Classic {#salesforce-classic}

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Klicken Sie auf **Setup** > **Build** > **Anpassen** > **Aktivitäten** > **Aufgabenfelder**.
1. Klicken Sie auf **Typ**.
1. Klicken Sie unter &quot;Task Type Picklist Value&quot;auf **New**.
1. Geben Sie den Namen der fehlenden Task Type Picklist-Werte ein (&quot;E-Mail, &quot;Aufruf&quot;, &quot;Antwort&quot;).
1. Klicken Sie auf **Speichern**.

Nachdem dies eingerichtet ist, sehen Sie, wie das Feld Typ den entsprechenden Wert für aufgezeichnete E-Mails, Aufrufe und Antworten enthält. Diese Werte werden bei Erinnerungsaufgaben für Sales Insight-Aktionen _nicht_ ausgefüllt.

>[!NOTE]
>
>Wenn Sie &quot;Antwort&quot;nicht als Wert sehen, fügen Sie ihn hinzu, indem Sie auf **Neu** klicken. &quot;Antwort&quot;ist kein Standardwert in Salesforce.

>[!MORELIKETHIS]
>
>* [Protokollieren von Attributen zu Verkaufsaktivitäten in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Konfigurieren der Anpassung der Details der Salesforce-Aktivität](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Vertriebsaktivitäten mit Salesforce synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
