---
description: Synchronisieren von Abmeldungen mit Salesforce - Marketo Docs - Produktdokumentation
title: Synchronisieren von Abmeldungen mit Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: f174cba33e18812ac08adf177302d997bbe60c4c
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 5%

---

# Synchronisieren von Abmeldungen mit Salesforce {#syncing-unsubscribes-with-salesforce}

## Voraussetzungen für Abmeldungen zur Synchronisierung mit Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synchronisierung des Abmeldes muss aktiviert sein (für nächtliche Synchronisation)
* Das Feld Opt-out muss in Salesforce installiert sein.
* Personendatensätze in Marketo Sales müssen über eine Salesforce-ID verfügen

**Push-Abmeldungen**

Wenn eine Abmeldung in Marketo Sales erfasst wird, senden wir sie in Echtzeit an Salesforce und aktualisieren eines der Opt-out-Felder, mit denen Sie die Synchronisation ausgewählt haben. Wenn Sie die Salesforce-Synchronisation deaktiviert haben, werden wir die Abmeldung weiterhin an die E-Mail-Abmeldung weiterleiten.

**Abmeldesynchronisierung**

Wenn Sie die Synchronisation zum Abmelden aktiviert haben (Schritt 3 unten), wird die nächtliche Synchronisation aktiviert. Die Synchronisierung findet einmal täglich um 20:00 Uhr PST statt. Dadurch werden alle Abmeldungen in Marketo Sales bidirektional mit dem Opt-out-Feld in Salesforce synchronisiert.

## Konfigurieren der Abmeldesynchronisierung mit Salesforce {#configure-unsubscribe-sync-to-salesforce}

Benutzer können entscheiden, ob sie ihre Abmeldungen mit dem standardmäßigen Feld für die E-Mail-Abmeldung synchronisieren möchten, mit dem Marketo auch synchronisieren kann, oder sie können mit dem Feld für die Marketo-Abmeldung für Vertrieb synchronisieren, sodass zwischen Abmeldungen für Vertrieb und Abmeldungen für Marketing unterschieden werden kann.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Abmeldungen**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Klicken Sie auf **Integrationen** Registerkarte. Aktivieren Sie unter Mit Salesforce synchronisieren die nächtliche Synchronisierung.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Wählen Sie das Feld aus, mit dem Sie synchronisieren möchten.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Feld | Beschreibung |
   |---|---|
   | **Abmeldefeld Synchronisieren mit Sales Force** | Standardmäßig ausgewählt, wird nur das Feld Salesforce Opt-out aktualisiert. |
   | **Synchronisierung mit Marketo Sales Opt Out-Feld** | Wenn Sie die Abmeldungen für Vertrieb und Marketing trennen möchten, wählen Sie diese Option, um zusätzliche [Marketo Sales Opt-out-Feld.](#msoo) |

## Installieren des Felds &quot;Opt-out&quot;im Seitenlayout {#installing-the-opt-out-field-in-the-page-layout}

**E-Mail-Abmeldung**

Email Opt-out ist ein Standardfeld in Salesforce, das über Salesforce installiert werden kann. Sie müssen Salesforce-Administrator sein, um es zu installieren.

1. Navigieren Sie zu [Salesforce.com](https://salesforce.com) und melden Sie sich an.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Klicken Sie auf Ihren Benutzernamen und wählen Sie **Einrichtung**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Suchen Sie im Schnellsuchfeld nach Kontakt oder Lead. In diesem Szenario installieren wir das Feld im Layout Kontaktseite , aber Sie sollten es für beide Personendatensätze installieren.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Auswählen **Seitenlayouts**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Auswählen **Bearbeiten** neben dem Seitenlayout, dem Sie das Feld hinzufügen möchten.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Auswählen **Felder**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Ziehen Sie E-Mail-Opt-out per Drag-and-Drop in das Seitenlayout.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Klicken **Speichern**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Abmeldung von Marketo Sales {#marketo-sales-opt-out}

Das Marketo Sales Opt-out-Feld ist ein benutzerdefiniertes Feld, das Benutzern zur Verfügung steht, die das Marketo Sales Insight-Paket installiert haben. [von der AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

Nachdem Sie das Marketo Sales Insight-Paket von der AppExchange in Salesforce erfolgreich installiert haben, sehen Sie das für Sie verfügbare Feld Marketo Sales Opt-out .
