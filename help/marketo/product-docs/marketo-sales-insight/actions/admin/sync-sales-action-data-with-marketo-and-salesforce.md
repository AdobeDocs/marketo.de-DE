---
description: Synchronisieren von Verkaufsaktionsdaten mit Marketo und Salesforce - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren von Verkaufsaktionsdaten mit Marketo und Salesforce
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 4%

---

# Synchronisieren von Verkaufsaktionsdaten mit Marketo und Salesforce {#sync-sales-action-data-with-marketo-and-salesforce}

Mit der Feldsynchronisierung zur Datenvereinheitlichung für Sales Insight Actions kann das System Personeninformationen aus Ihrer Marketo Engage-Datenbank in Ihre Sales Insight Actions-Datenbank abrufen.

Dadurch werden aktuelle Personendaten in der Web-App für Sales Insight Actions bereitgestellt und das System kann eindeutige IDs für entsprechende Personendatensätze in Marketo und Lead-/Kontakt-/Konto-/Opportunity-Datensätze in Salesforce erfassen, sodass Datensätze für die Protokollierung von Daten ordnungsgemäß referenziert werden können.

Diese Synchronisierung kann über die Registerkarte Sales Insight Actions Config im Abschnitt Admin von Marketo Engage aktiviert werden. Weitere Informationen finden Sie unter [Datensynchronisierung starten](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Das obige Diagramm zeigt, wie Daten zu Personenaktivitäten und Aufgaben zwischen Systemen synchronisiert werden können. Beachten Sie Folgendes:

* Personendatensätze werden mit Insight-Verkaufsaktionen aus Marketo Engage synchronisiert, wodurch Marketo Engage zur Wahrheitsquelle für Personen-Daten zu Insight-Verkaufsaktionen wird
* Sowohl Marketo Engage- als auch Sales Insight[Aktionen verfügen über einen Mechanismus](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) zum Erfassen und Synchronisieren des Abmeldestatus mit Salesforce
* Der Abmeldestatus wird nicht mit Verkaufsaktionen für Marketo Engage synchronisiert. Sales Insight-Aktionen können jedoch so konfiguriert werden, dass der Marketo-Abmeldestatus von Personen überprüft wird, bevor Verkäufern erlaubt wird, eine E-Mail mit der [Marketo-Abmeldeprüfung](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md) zu senden.

Im Folgenden finden Sie einige häufig gestellte Fragen zur Funktionsweise der Datenvereinheitlichungssynchronisierung.

## Welche Leads/Kontakte werden mit Sales Insight-Aktionen synchronisiert? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Leads und Kontakte, denen ein Vertriebsverantwortlicher zugewiesen ist, werden mit Verkaufsaktionen synchronisiert.

Sie können sehen, ob ein Lead/Kontakt über einen Vertriebsinhaber in Salesforce verfügt, indem Sie das Feld „Standardinhaber“ überprüfen.

Der Verkaufsinhaber muss nicht der Marketo-Synchronisierungsbenutzer oder ein bestimmter Salesforce- oder Verkaufsbenutzer sein. Wir benötigen lediglich eine Benutzerin bzw. einen Benutzer, die bzw. der im Feld „Lead-Inhaber“ und „Kontaktinhaber“ in Salesforce aufgeführt ist. Auf diese Weise können wir die Person als Vertriebs-Lead identifizieren und mit Insight-Aktionen für den Vertrieb synchronisieren. Alle Aktualisierungen der Felder, mit denen wir synchronisieren, werden auch in Sales Insight Actions erkannt und aktualisiert.

## Woher werden die Aktivitätsdaten, die im Smart Grid von Sales Insight angezeigt werden, bezogen? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Die Aktivitätsdaten wie E-Mail, Anruf, Interessante Momente und Web stammen alle aus der Marketo Engage-Datenbank. Das Smart Grid von Sales Insight stellt eine Anfrage an die Marketo Engage-Instanz, um diese jedes Mal abzurufen, wenn ein Vertriebsbenutzer das Bedienfeld Sales Insight lädt.

![](assets/actions-data-sync-faq-4.png)

Um sicherzustellen, dass alle Aktivitätsdaten aus Marketo Engage bezogen werden können, synchronisiert Sales Insight Actions alle Aktivitätsdaten mit Marketo Engage.

## Welche Felder, die sich auf Personendatensätze beziehen, werden von Marketo Engage mit Insight-Verkaufsaktionen synchronisiert? {#what-fields-sync}

Es gibt 11 Felder, die von Marketo Engage mit Insight Sales-Aktionen synchronisiert werden:

* Vorname
* Last name
* Salesforce Kontakt-ID
* Salesforce Lead-ID
* Salesforce-Konto-ID
* Salesforce Opportunity-ID
* Marketo-ID
* Unternehmen
* Titel
* E-Mail
* Telefonnummer
* LinkedIn-URL
* Quelle

## Sind die Felder, die zwischen Marketo Engage- und Sales Insight-Aktionen synchronisieren, konfigurierbar? {#are-the-fields-that-sync-configurable}

Es ist nicht verfügbar, zu konfigurieren, welche Marketo Engage-Felder mit Sales Insight-Aktionen synchronisiert werden, und es ist auch nicht möglich, Felder zuzuordnen. Die Synchronisierung von Marketo ordnet standardmäßige Marketo-Felder automatisch Standardfeldern in Ihrer Sales Action-Instanz zu.

## Warum verfügt Sales Insight Actions über eine eigene Datenbank? {#why-does-actions-have-its-own-database}

Sales Insight Actions verfügt über eine eigene Web-Anwendung mit einer dedizierten Personen- und Aktivitätsdatenbank, um einen optimierten Arbeitsbereich bereitzustellen, der für Vertriebsteams entwickelt und konzipiert wurde. So haben Vertriebsleiter und Verkäufer einen Raum, um ihre Interaktionsstrategie zu entwickeln und zu verwalten   ohne Zugriff oder Berechtigungen auf den primären Marketo Engage-Arbeitsbereich zu gewähren, der für Experten für Marketing-Vorgänge optimiert ist.

## Wie werden Duplikate behandelt? {#how-are-duplicates-handled}

Ihre Sales Actions-Datenbank ist eine Kopie der qualifizierten Personen (Leads/Kontakte mit einem Sales Owner), die in Ihrer Marketo Engage-Datenbank vorhanden sind. Wenn also zwei Datensätze mit derselben E-Mail-Adresse in Marketo erstellt wurden, wird in Verkaufsaktionen ein doppelter Datensatz erstellt.

## Wie lange dauert es, bis die erste Synchronisierung abgeschlossen ist? {#how-long-initial-sync}

Der anfängliche Prozess zum Synchronisieren aller Ihrer Vertriebs-Lead-Daten mit einer neuen Sales Insight Actions-Instanz verarbeitet Personen in der Regel alle 1-2 Minuten mit etwa 1.000 Personen. Dies ist nur eine Schätzung und kann variieren.

Sobald die Erstsynchronisierung stattfindet und alle Ihre Vertriebs-Leads in Ihre Web-App-Instanz für Sales Insight Actions eingefügt wurden, findet eine inkrementelle Synchronisierung statt, die jedes Mal ausgeführt wird, wenn eines der unterstützten Felder aktualisiert wird, die synchronisiert werden.

## Können Benutzer von Sales Insight-Aktionen Personendaten über die Web-App für Aktionen bearbeiten? {#can-actions-users-edit-people-data}

Nein, die Möglichkeit, Personendatensätze in Aktionen zu erstellen und zu bearbeiten, ist sowohl für Benutzer als auch für Administratoren der Aktionswebanwendung nicht verfügbar. Das Erstellen und Bearbeiten von Personen muss entweder in Salesforce oder Marketo Engage erfolgen. Sales Insight Actions verwendet Marketo als Datenquelle für Personendaten, indem kontinuierlich neue Daten synchronisiert werden. Wenn also eine Person in Marketo entweder über einen Workflow in Marketo aktualisiert oder von Salesforce synchronisiert wird, werden diese Aktualisierungen an die Sales Insight Actions Web App-Datenbank übergeben.

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

## Loggen sich Vertriebsaktivitäten in Salesforce ein? {#do-sales-activities-log-to-salesforce}

Ja, die Vertriebsaktivitäten werden in Salesforce als native Aufgaben protokolliert. Diese Aufgaben können dann in Salesforce-Berichten verwendet werden, um Team-Dashboards zur Verfolgung von Vertriebsaktivitäten zu betreiben.

Mit Sales Insight-Aktionen können Administratoren konfigurieren, welche Verkaufsaktivitäten in Salesforce protokolliert werden. Zu diesen Aktivitäten gehören E-Mails, Aufrufe und offene Erinnerungsaufgaben.

![](assets/actions-data-sync-faq-6.png)

Das obige Diagramm zeigt, welche Informationen in Salesforce protokolliert werden. Aktivitäten wie E-Mails und Anrufe werden in Salesforce in einer [&#x200B; (unidirektionalen Synchronisation) &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). [Abmeldungen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) und [Erinnerungsaufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) werden mit einer bidirektionalen Synchronisation auf dem neuesten Stand gehalten. Jede dieser Datensynchronisationen kann über die Web-App-Oberfläche der Sales Insight Actions konfiguriert werden.

>[!MORELIKETHIS]
>
>* [Abmeldungen mit Salesforce synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo-Abmeldeprüfung](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Verkaufsaktivitäten mit Salesforce synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Erinnerungsaufgabe - Synchronisieren mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Initiieren der Datensynchronisation](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
