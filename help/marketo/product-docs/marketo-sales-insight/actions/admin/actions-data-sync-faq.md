---
description: Häufig gestellte Fragen zur Datensynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Datensynchronisation von Aktionen
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26173379c89393596b3ece18c7f7e945a79588d9
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 3%

---

# Häufig gestellte Fragen zur Datensynchronisation von Aktionen {#actions-data-sync-faq}

Die Datenzusammenführungsfeldsynchronisierung für Sales Insight-Aktionen ermöglicht es dem System, personenbezogene Daten aus Ihrer Marketo Engage-Datenbank in Ihre Sales Insight-Aktionsdatenbank zu übertragen.

Dadurch werden in der Web-App Sales Insight-Aktionen aktuelle Personendaten bereitgestellt und das System kann eindeutige IDs für die entsprechenden Personendatensätze in Marketo und Lead-/Kontakt-/Konto-/Opportunity-Datensätze in Salesforce erfassen, sodass Datensätze ordnungsgemäß für die Protokollierung von Daten referenziert werden können.

Diese Synchronisierung kann über die Registerkarte Konfiguration von Sales Insight-Aktionen im Admin-Bereich von Marketo Engage aktiviert werden. Weitere Informationen finden Sie unter [Datensynchronisation starten](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Das obige Diagramm zeigt, wie Personen-Aktivitäten und Aufgabendaten zwischen Systemen synchronisiert werden können. Beachten Sie Folgendes:

* Personendatensätze werden mit Sales Insight-Aktionen von Marketo Engage synchronisiert, wodurch Marketo Engage zur &quot;Source of Truth&quot; für Sales Insight-Aktionen und Personendaten wird
* Marketo Engage- und Sales Insight-Aktionen [über einen Mechanismus verfügen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) zur Erfassung und Synchronisierung des Abmeldestatus für Salesforce
* Der Status Abmelden wird nicht von Verkaufsaktionen mit Marketo Engage synchronisiert, aber Sales Insight-Aktionen können so konfiguriert werden, dass der Marketo-Abmeldestatus von Personen überprüft wird, bevor Verkäufern gestattet wird, eine E-Mail mit [Prüfung der Marketo-Abmeldung](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Im Folgenden finden Sie einige häufig gestellte Fragen zur Funktionsweise der Synchronisierung von Daten.

## Welche Leads/Kontakte werden mit Sales Insight-Aktionen synchronisiert? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Leads und Kontakte, denen ein Vertriebseigentümer zugewiesen ist, werden in Verkaufsaktionen synchronisiert.

Sie können sehen, ob ein Lead/Kontakt in Salesforce über einen Verkaufsinhaber verfügt, indem Sie sich das Standardeigentümerfeld ansehen.

Der Vertriebsinhaber muss nicht der Marketo-Synchronisierungsbenutzer oder ein bestimmter Salesforce- oder Vertriebsbenutzer sein. Alles, was wir benötigen, ist, dass ein Benutzer im Feld Lead-Eigentümer und Kontaktbesitzer in Salesforce aufgelistet ist, damit wir ihn als Verkaufsleiter identifizieren und mit Sales Insight-Aktionen synchronisieren können. Sämtliche Aktualisierungen der Felder, mit denen wir synchronisieren, werden ebenfalls in Sales Insight-Aktionen erkannt und aktualisiert.

## Woher werden die im Smart Grid von Sales Insight angezeigten Aktivitätsdaten abgerufen? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Die Aktivitätsdaten wie E-Mail, Anruf, interessanter Moment und Web werden alle aus der Marketo Engage-Datenbank abgerufen. Das Smart Grid für Sales Insight stellt eine Anfrage an die Marketo Engage-Instanz, diese jedes Mal abzurufen, wenn ein Vertriebsbenutzer das Bedienfeld Sales Insight lädt.

![](assets/actions-data-sync-faq-4.png)

Um sicherzustellen, dass alle Aktivitätsdaten von Marketo Engage bezogen werden können, synchronisiert Sales Insight Actions alle Aktivitätsdaten mit Marketo Engage.

## Welche Felder beziehen sich auf Personendatensätze, die von Marketo Engage zu Sales Insight-Aktionen synchronisiert werden? {#what-fields-sync}

Es gibt 11 Felder, die von Marketo Engage mit Sales Insight-Aktionen synchronisiert werden:

* Vorname
* Nachname
* Salesforce-Kontakt-ID
* Salesforce-Lead-ID
* Salesforce-Konto-ID
* Salesforce Opportunity ID
* Marketo-ID
* Unternehmen
* Titel
* E-Mail
* Telefonnummer
* LinkedIn-URL
* Quelle

## Sind die Felder, die zwischen Marketo Engage und Sales Insight-Aktionen synchronisiert werden, konfigurierbar? {#are-the-fields-that-sync-configurable}

Es ist nicht möglich, zu konfigurieren, welche Marketo Engage-Felder mit Sales Insight-Aktionen synchronisiert werden, und auch keine Felder zuzuordnen. Die Synchronisierung von Marketo ordnet Marketo-Standardfelder automatisch den Standardfeldern in Ihrer Verkaufsaktionsinstanz zu.

## Warum verfügen Sales Insight-Aktionen über eine eigene Datenbank? {#why-does-actions-have-its-own-database}

Sales Insight Actions verfügt über eine eigene Webanwendung mit einer dedizierten Personen- und Aktivitätsdatenbank, um einen optimierten Arbeitsbereich bereitzustellen, der für Verkaufsteams erstellt und entwickelt wurde. Dies ermöglicht es Vertriebsmitarbeitern und Verkäufern, ihre Interaktionsstrategie zu entwickeln und zu verwalten, ohne Zugriff oder Berechtigungen auf den primären Marketo Engage Workspace zu gewähren, der für Marketingoperationsspezialisten optimiert ist.

## Wie werden Duplikate behandelt? {#how-are-duplicates-handled}

Ihre Verkaufsaktionsdatenbank ist eine Kopie der qualifizierten Personen (Leads/Kontakte mit einem Vertriebsmitarbeiter), die in Ihrer Marketo Engage-Datenbank vorhanden sind. Wenn also zwei Datensätze mit derselben E-Mail-Adresse in Marketo erstellt werden, wird in Verkaufsaktionen ein doppelter Datensatz erstellt.

## Wie lange dauert es, bis die erste Synchronisierung abgeschlossen ist? {#how-long-initial-sync}

Der anfängliche Prozess für die Synchronisierung aller Ihrer Verkaufs-Lead-Daten in einer neuen Sales Insight-Aktionsinstanz verarbeitet in der Regel Personen in etwa 1.000 Fällen alle 1 bis 2 Minuten. Dies ist nur eine Schätzung und kann variieren.

Sobald die erste Synchronisierung stattgefunden hat und alle Ihre Verkaufs-Leads in Ihrer Web-App-Instanz mit Sales Insight-Aktionen gefüllt wurden, wird eine inkrementelle Synchronisierung ausgeführt, die jedes Mal ausgeführt wird, wenn eine Aktualisierung auf eines der unterstützten Felder durchgeführt wird, die synchronisiert werden.

## Können Benutzer von Sales Insight-Aktionen Personendaten aus der Web-App &quot;Aktionen&quot;bearbeiten? {#can-actions-users-edit-people-data}

Nein, die Möglichkeit, Personendatensätze in Aktionen zu erstellen und zu bearbeiten, ist für Benutzer und Administratoren der Web-App &quot;Aktionen&quot;nicht verfügbar. Das Erstellen und Bearbeiten von Personen muss entweder in Salesforce oder im Marketo Engage erfolgen. Sales Insight Actions verwendet Marketo als &quot;Source of Truth&quot; für Personendaten, indem sie kontinuierlich neue Daten synchronisieren. Wenn eine Person also entweder über einen Workflow in Marketo aktualisiert oder in Marketo erstellt oder über Salesforce synchronisiert wird, werden diese Aktualisierungen an die Web-App-Datenbank für Sales Insight-Aktionen weitergeleitet.

## Protokollieren Verkaufsaktivitäten Marketo? {#do-sales-activities-log-to-marketo}

Ja, die Aktivitäten zur Verkaufsinteraktion melden sich bei Marketo als native Aktivitäten an. Diese Aktivitäten enthalten auch native Filter, die mit Einschränkungen verwendet werden können, um Leads basierend auf Attributen der Verkaufsaktivität auszuwählen.

![](assets/actions-data-sync-faq-5.png)

Nachstehend finden Sie eine Liste der Aktivitäten, die sich bei Marketo anmelden:

* Verkaufs-E-Mail senden
* Verkaufs-E-Mail öffnen
* Auf Verkaufs-E-Mail klicken
* Hat auf Vertriebsemail geantwortet
* Verkaufs-E-Mail war aufgrund eines Bounce-Ereignisses unzustellbar
* Verkaufsaufruf empfangen
* Zur Verkaufskampagne hinzufügen
* Aus Verkaufskampagne entfernt

## Protokollieren Verkaufsaktivitäten Salesforce? {#do-sales-activities-log-to-salesforce}

Ja, Verkaufsaktivitäten melden sich als native Aufgaben bei Salesforce an. Diese Aufgaben können dann in Salesforce-Berichten verwendet werden, um Team-Dashboards zu unterstützen, die Vertriebsaktivitäten verfolgen.

Mit Sales Insight-Aktionen können Administratoren konfigurieren, welche Verkaufsaktivitäten bei Salesforce protokolliert werden. Zu diesen Aktivitäten gehören E-Mails, Aufrufe und offene Erinnerungsaufgaben.

![](assets/actions-data-sync-faq-6.png)

Das obige Diagramm zeigt, welche Informationen bei Salesforce protokolliert werden. Aktivitäten wie E-Mails und Aufrufe werden in Salesforce in einer [unidirektionale Synchronisation](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Abmeldungen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) und [Erinnerungsaufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) werden mit einer bidirektionalen Synchronisation auf dem neuesten Stand gehalten. Jede dieser Datensynchronisierungen kann über die Web-App-Oberfläche der Sales Insight-Aktionen konfiguriert werden.

>[!MORELIKETHIS]
>
>* [Synchronisieren von Abmeldungen mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Prüfung der Marketo-Abmeldung](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Salesforce-Synchronisierungseinstellungen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Erinnern von Aufgabensynchronisierung mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Datensynchronisation starten](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

