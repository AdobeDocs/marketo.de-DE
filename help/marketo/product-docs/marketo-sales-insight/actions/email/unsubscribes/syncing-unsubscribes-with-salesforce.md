---
description: Synchronisieren von Abmeldungen mit Salesforce - Marketo Docs - Produktdokumentation
title: Synchronisieren von Abmeldungen mit Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Synchronisieren von Abmeldungen mit Salesforce {#syncing-unsubscribes-with-salesforce}

Wenn Sie Abmeldungen mit einem Opt-out-Feld in Salesforce synchronisieren möchten, können Sie die Salesforce-Abmelde-Synchronisation verwenden.

## Voraussetzungen für Abmeldungen zur Synchronisierung mit Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synchronisierung des Abmeldes muss aktiviert sein (für nächtliche Synchronisation)
* Das Feld Opt-out muss in Salesforce installiert sein.
* Personendatensätze in Marketo Sales müssen über eine Salesforce-ID verfügen

**Push unsubscribes**

Wenn eine Abmeldung in Marketo Sales erfasst wird, senden wir sie in Echtzeit an Salesforce und aktualisieren eines der Opt-out-Felder, mit denen Sie die Synchronisation ausgewählt haben. Wenn Sie die Salesforce-Synchronisation deaktiviert haben, werden wir die Abmeldung weiterhin an die E-Mail-Abmeldung weiterleiten.

**Synchronisation abmelden**

Wenn Sie die Synchronisation zum Abmelden aktiviert haben (Schritt 3 unten), wird die nächtliche Synchronisation aktiviert. Die Synchronisierung findet einmal täglich um 20:00 Uhr PST statt. Dadurch werden alle Abmeldungen in Marketo Sales bidirektional mit dem Opt-out-Feld in Salesforce synchronisiert.

>[!NOTE]
>
>Die Synchronisierung der Abmeldung mit Salesforce synchronisiert Abmeldungen, synchronisiert aber keine erneuten Abonnenten. Wenn Sie eine Abmeldung von Marketo Sales und Salesforce entfernen möchten, deaktivieren Sie die Abmeldung in Salesforce und entfernen Sie die Abmeldung in Marketo Sales.

## Konfigurieren der Abmeldesynchronisierung mit Salesforce {#configure-unsubscribe-sync-to-salesforce}

Benutzer können entscheiden, ob sie ihre Abmeldungen mit dem standardmäßigen Feld für die E-Mail-Abmeldung synchronisieren möchten, mit dem Marketo auch synchronisieren kann, oder sie können mit dem Feld für die Marketo-Abmeldung für Vertrieb synchronisieren, sodass zwischen Abmeldungen für Vertrieb und Abmeldungen für Marketing unterschieden werden kann.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Unsubscribes**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Klicken Sie auf die Registerkarte **Integrationen**. Aktivieren Sie unter Mit Salesforce synchronisieren die nächtliche Synchronisierung.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Wählen Sie das Feld aus, mit dem Sie synchronisieren möchten.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Feld | Beschreibung |
   |---|---|
   | **Mit Salesforce-Opt-out-Feld synchronisieren** | Standardmäßig ausgewählt, wird nur das Feld Salesforce Opt-out aktualisiert. |
   | **Mit Marketo Sales Opt-out-Feld synchronisieren** | Wenn Sie die Abmeldungen für Vertrieb und Marketing trennen möchten, wählen Sie diese Option, um das zusätzliche Feld für die Abmeldung von Marketo-Verkäufen zu aktualisieren.](#msoo)[ |

## Installieren des Felds &quot;Opt-out&quot;im Seitenlayout {#installing-the-opt-out-field-in-the-page-layout}

**E-Mail-Opt-out**

Email Opt-out ist ein Standardfeld in Salesforce, das über Salesforce installiert werden kann. Sie müssen Salesforce-Administrator sein, um es zu installieren.

1. Gehen Sie zu [Salesforce.com](https://salesforce.com) und melden Sie sich an.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Klicken Sie auf Ihren Benutzernamen und wählen Sie **Einrichten** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Suchen Sie im Schnellsuchfeld nach Kontakt oder Lead. In diesem Szenario installieren wir das Feld im Layout Kontaktseite , aber Sie sollten es für beide Personendatensätze installieren.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Wählen Sie **Seitenlayouts** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Wählen Sie neben dem Seitenlayout, dem Sie das Feld hinzufügen möchten, die Option **Bearbeiten** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Wählen Sie **Felder** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Ziehen Sie E-Mail-Opt-out in das Seitenlayout.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Abmeldung von Marketo Sales {#marketo-sales-opt-out}

Das Marketo Sales Opt-out -Feld ist ein benutzerdefiniertes Feld, das Benutzern zur Verfügung steht, die das Marketo Sales Insight-Paket [über die AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} installiert haben.

Nachdem Sie das Marketo Sales Insight-Paket von der AppExchange in Salesforce erfolgreich installiert haben, sehen Sie das für Sie verfügbare Feld Marketo Sales Opt-out .
