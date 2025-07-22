---
description: Häufig gestellte Fragen zur Datensynchronisierung für Aktionen - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Datensynchronisation für Aktionen
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%

---

# Häufig gestellte Fragen zur Datensynchronisation für Aktionen {#actions-data-sync-faq}

Mit der Feldsynchronisierung zur Datenvereinheitlichung für [!DNL Sales Insight Actions] kann das System Personeninformationen aus Ihrer Marketo Engage-Datenbank in Ihre [!DNL Sales Insight Actions]-Datenbank abrufen.

Dadurch werden aktuelle Personendaten in der [!DNL Sales Insight Actions]-Web-App bereitgestellt und das System kann eindeutige IDs für entsprechende Personendatensätze in Marketo und Lead-/Kontakt-/Konto-/Opportunity-Datensätze in [!DNL Salesforce] erfassen, sodass Datensätze für die Protokollierung von Daten ordnungsgemäß referenziert werden können.

Diese Synchronisierung kann über die Registerkarte [!DNL Sales Insight Actions] im Abschnitt Admin von Marketo Engage aktiviert werden. Weitere Informationen finden Sie unter [Datensynchronisierung starten](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Das obige Diagramm zeigt, wie Daten zu Personenaktivitäten und Aufgaben zwischen Systemen synchronisiert werden können. Beachten Sie Folgendes:

* Personendatensätze werden mit [!DNL Sales Insight Actions] aus Marketo Engage synchronisiert, sodass Marketo Engage die Datenquelle für [!DNL Sales Insight Actions] Personendaten ist
* Sowohl Marketo Engage als auch [!DNL Sales Insight Actions] [verfügen über einen Mechanismus](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) zum Erfassen und Synchronisieren des Abmeldestatus mit [!DNL Salesforce]
* Der Abmeldestatus wird nicht mit Verkaufsaktionen für Marketo Engage synchronisiert. [!DNL Sales Insight Actions] kann jedoch so konfiguriert werden, dass der Marketo-Abmeldestatus von Personen geprüft wird, bevor Verkäufern erlaubt wird, eine E-Mail mit der [Marketo-Abmeldeprüfung zu ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Im Folgenden finden Sie einige häufig gestellte Fragen zur Funktionsweise der Datenvereinheitlichungssynchronisierung.

## Welche Leads/Kontakte werden mit [!DNL Sales Insight Actions] synchronisiert? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Leads und Kontakte, denen ein Vertriebsverantwortlicher zugewiesen ist, werden mit Verkaufsaktionen synchronisiert.

Sie können sehen, ob ein Lead/Kontakt einen Vertriebsmitarbeiter in [!DNL Salesforce] hat, indem Sie das Feld „Standardbesitzer“ überprüfen, das vorhanden ist.

Der Verkaufsinhaber muss nicht der Marketo-Synchronisierungsbenutzer oder ein bestimmter [!DNL Salesforce] oder Verkaufsbenutzer sein. Wir benötigen lediglich einen Benutzer, der im Feld Lead-Inhaber und Kontaktinhaber in [!DNL Salesforce] aufgeführt ist, damit wir ihn als Vertriebs-Lead identifizieren und mit [!DNL Sales Insight Actions] synchronisieren können. Alle Aktualisierungen der Felder, mit denen wir synchronisieren, werden ebenfalls in [!DNL Sales Insight Actions] erkannt und aktualisiert.

## Woher werden die Aktivitätsdaten, die im Smart Grid von Sales Insight angezeigt werden, bezogen? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Die Aktivitätsdaten wie E-Mail, Anruf, Interessante Momente und Web stammen alle aus der Marketo Engage-Datenbank. Das Smart Grid von Sales Insight stellt eine Anfrage an die Marketo Engage-Instanz, um diese jedes Mal abzurufen, wenn ein Vertriebsbenutzer das Bedienfeld Sales Insight lädt.

![](assets/actions-data-sync-faq-4.png)

Um sicherzustellen, dass alle Aktivitätsdaten aus Marketo Engage bezogen werden können, synchronisiert [!DNL Sales Insight Actions] alle Aktivitätsdaten mit Marketo Engage.

## Welche Felder, die sich auf Personendatensätze beziehen, werden von Marketo Engage mit [!DNL Sales Insight Actions] synchronisiert? {#what-fields-sync}

Es gibt 11 Felder, die von Marketo Engage mit [!DNL Sales Insight Actions] synchronisiert werden:

* Vorname
* Last name
* [!DNL Salesforce] Kontakt-ID
* Lead-ID [!DNL Salesforce]
* [!DNL Salesforce] Konto-ID
* Opportunity-ID [!DNL Salesforce]
* Marketo-ID
* Unternehmen
* Titel
* E-Mail
* Telefonnummer
* [!DNL Linkedin] URL
* Quelle

## Sind die Felder, die zwischen Marketo Engage und [!DNL Sales Insight Actions] synchronisiert werden, konfigurierbar? {#are-the-fields-that-sync-configurable}

Es ist nicht möglich, zu konfigurieren, welche Marketo Engage-Felder mit [!DNL Sales Insight Actions] synchronisiert werden sollen, und auch nicht, Felder zuzuordnen. Die Synchronisierung von Marketo ordnet standardmäßige Marketo-Felder automatisch Standardfeldern in Ihrer Sales Action-Instanz zu.

## Warum hat [!DNL Sales Insight Actions] eine eigene Datenbank? {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] verfügt über eine eigene Web-Anwendung mit einer dedizierten Personen- und Aktivitätsdatenbank, um einen optimierten Arbeitsbereich bereitzustellen, der für Vertriebsteams erstellt und entwickelt wurde. So haben Vertriebsleiter und Verkäufer einen Raum, um ihre Interaktionsstrategie zu entwickeln und zu verwalten   ohne Zugriff oder Berechtigungen auf den primären Marketo Engage-Arbeitsbereich zu gewähren, der für Experten für Marketing-Vorgänge optimiert ist.

## Wie werden Duplikate behandelt? {#how-are-duplicates-handled}

Ihre Sales Actions-Datenbank ist eine Kopie der qualifizierten Personen (Leads/Kontakte mit einem Sales Owner), die in Ihrer Marketo Engage-Datenbank vorhanden sind. Wenn also zwei Datensätze mit derselben E-Mail-Adresse in Marketo erstellt wurden, wird in Verkaufsaktionen ein doppelter Datensatz erstellt.

## Wie lange dauert es, bis die erste Synchronisierung abgeschlossen ist? {#how-long-initial-sync}

Der anfängliche Prozess zum Synchronisieren aller Ihrer Vertriebs-Lead-Daten mit einer neuen [!DNL Sales Insight Actions]-Instanz verarbeitet in der Regel Personen mit etwa 1.000 Kontakten alle 1-2 Minuten. Dies ist nur eine Schätzung und kann variieren.

Sobald die Erstsynchronisierung stattfindet und alle Ihre Vertriebs-Leads in Ihre [!DNL Sales Insight Actions]-Web-App-Instanz eingefügt wurden, wird eine inkrementelle Synchronisierung durchgeführt, die jedes Mal ausgeführt wird, wenn eines der unterstützten Felder aktualisiert wird, die synchronisiert werden.

## Können [!DNL Sales Insight Actions] Benutzer Personendaten über die Web-App „Aktionen“ bearbeiten? {#can-actions-users-edit-people-data}

Nein, die Möglichkeit, Personendatensätze in Aktionen zu erstellen und zu bearbeiten, ist sowohl für Benutzer als auch für Administratoren der Aktionswebanwendung nicht verfügbar. Das Erstellen und Bearbeiten von Personen muss in [!DNL Salesforce] oder Marketo Engage erfolgen. [!DNL Sales Insight Actions] verwendet Marketo als Datenquelle für Personendaten, indem kontinuierlich neue Daten synchronisiert werden. Wenn also eine Person in Marketo entweder über einen Workflow in Marketo aktualisiert oder aus [!DNL Salesforce] synchronisiert wird, werden diese Aktualisierungen an die [!DNL Sales Insight Actions] Web-App-Datenbank übergeben.

## Loggen sich Vertriebsaktivitäten in Marketo ein? {#do-sales-activities-log-to-marketo}

Ja, die Vertriebsaktivitäten werden in Marketo als native Aktivitäten protokolliert. Diese Aktivitäten enthalten auch native Filter, die mit Einschränkungen verwendet werden können, um Leads basierend auf Attributen der Verkaufsaktivität anzusprechen.

![](assets/actions-data-sync-faq-5.png)

Nachfolgend finden Sie eine Liste der Aktivitäten, die sich bei Marketo anmelden:

* Verkaufs-E-Mail senden
* Verkaufs-E-Mail öffnen
* Auf Verkaufs-E-Mail klicken
* Hat auf Vertriebsemail geantwortet
* Verkaufs-E-Mail war aufgrund eines Bounce-Ereignisses unzustellbar
* Verkaufsanruf empfangen
* Zur Verkaufskampagne hinzufügen
* Aus Verkaufskampagne entfernt

## Protokollieren sich Vertriebsaktivitäten bei [!DNL Salesforce]? {#do-sales-activities-log-to-salesforce}

Ja, Vertriebsaktivitäten werden in [!DNL Salesforce] als native Aufgaben protokolliert. Diese Aufgaben können dann in [!DNL Salesforce] Berichten verwendet werden, um Team-Dashboards zur Verfolgung von Vertriebsaktivitäten zu betreiben.

[!DNL Sales Insight Actions] können Administratoren konfigurieren, welche Vertriebsaktivitäten in [!DNL Salesforce] protokolliert werden. Zu diesen Aktivitäten gehören E-Mails, Aufrufe und offene Erinnerungsaufgaben.

![](assets/actions-data-sync-faq-6.png)

Das obige Diagramm zeigt, welche Informationen in [!DNL Salesforce] protokolliert werden. Aktivitäten wie E-Mails und Anrufe werden in [!DNL Salesforce] in einer [ Synchronisierung ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Abmeldungen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) und [Erinnerungsaufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) werden mit einer bidirektionalen Synchronisation auf dem neuesten Stand gehalten. Jede dieser Datensynchronisationen kann über [!DNL Sales Insight Actions] Web-App-Oberfläche konfiguriert werden.

>[!MORELIKETHIS]
>
>* [Abmeldungen werden synchronisiert mit [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo-Abmeldeprüfung](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] Einstellungen synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Erinnerungsaufgabe - Synchronisieren mit [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Initiieren der Datensynchronisation](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

