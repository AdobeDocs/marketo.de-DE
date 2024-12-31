---
description: Synchronisieren von Abmeldungen mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren von Abmeldungen mit Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Synchronisieren von Abmeldungen mit Salesforce {#syncing-unsubscribes-with-salesforce}

Wenn Sie Abmeldungen mit einem Opt-out-Feld in Salesforce synchronisieren möchten, können Sie die Salesforce-Abmeldesynchronisierung verwenden.

## Voraussetzungen für Abmeldungen zur Synchronisierung mit Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Abmeldesynchronisierung muss aktiviert sein (für die nächtliche Synchronisierung)
* Opt-out-Feld muss in Salesforce installiert sein
* Personendatensätze in Marketo Sales müssen eine Salesforce ID haben

**Push-Abmeldungen**

Wenn ein Abo-Abonnement in Marketo Sales erfasst wird, senden wir es in Echtzeit an Salesforce und aktualisieren eines der Opt-out-Felder, die Sie zur Synchronisierung ausgewählt haben. Wenn Sie die Salesforce-Synchronisierung deaktiviert haben, übertragen wir weiterhin die Abmeldung an die E-Mail-Abmeldung.

**Abo-Synchronisierung**

Wenn Sie die Abmeldesynchronisierung aktiviert haben (Schritt 3 unten), schalten Sie die nächtliche Synchronisierung ein. Die Synchronisierung erfolgt einmal täglich um 20:00 Uhr PST. Alle Abmeldungen in Marketo Sales werden bidirektional mit dem Opt-out-Feld in Salesforce synchronisiert.

>[!NOTE]
>
>Die Abmeldesynchronisierung mit Salesforce synchronisiert Abmeldungen, aber keine erneuten Abmeldungen. Wenn Sie ein Abo von Marketo Sales und Salesforce entfernen möchten, deaktivieren Sie das Kontrollkästchen Abo in Salesforce kündigen und entfernen Sie das Abo in Marketo Sales.

## Konfigurieren der Abmeldesynchronisierung mit Salesforce {#configure-unsubscribe-sync-to-salesforce}

Benutzerinnen und Benutzer können entscheiden, ob sie ihre Abmeldungen mit dem standardmäßigen E-Mail-Opt-out-Feld synchronisieren möchten, mit dem Marketo auch synchronisieren kann, oder sie können mit dem Marketo-Feld Verkaufsabmeldung synchronisieren, sodass Verkaufsabmeldungen und Marketing-Abmeldungen unterschieden werden können.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Wählen Sie unter Admin-Einstellungen **Abmeldungen** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Klicken Sie auf die **Integrationen**. Aktivieren Sie unter Mit Salesforce synchronisieren die nächtliche Synchronisierung.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Wählen Sie das Feld aus, mit dem Sie synchronisieren möchten.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Feld | Beschreibung |
   |---|---|
   | **Opt-out-Feld mit Salesforce synchronisieren** | Standardmäßig ausgewählt. Aktualisiert nur das Opt-out-Feld von Salesforce. |
   | **Feld „Mit Marketo Sales Opt-out synchronisieren“** | Wenn Sie Verkaufs- und Marketing-Abmeldungen trennen möchten, wählen Sie diese Option, um das zusätzliche Feld [Marketo-Verkaufsabmeldung zu aktualisieren.](#msoo) |

## Installieren des Opt-out-Felds im Seiten-Layout {#installing-the-opt-out-field-in-the-page-layout}

**E-Mail-Opt-out**

„E-Mail-Opt-out“ ist ein Standardfeld in Salesforce, das über Salesforce installiert werden kann. Sie müssen ein Salesforce-Administrator sein, um sie zu installieren.

1. Wechseln Sie zu [Salesforce.com](https://salesforce.com) und melden Sie sich an.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Klicken Sie auf Ihren Benutzernamen und wählen Sie **Setup**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Suchen Sie im Feld „Schnellsuche“ nach Kontakt oder Lead. In diesem Szenario installieren wir das Feld im Layout Kontaktseite , Sie sollten es jedoch für beide Personendatensätze installieren.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Wählen Sie **Seitenlayouts** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Klicken Sie **Bearbeiten** neben dem Seitenlayout, dem Sie das Feld hinzufügen möchten.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Wählen Sie **Felder** aus.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Ziehen Sie E-Mail-Opt-out per Drag-and-Drop in das Seiten-Layout.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Abmeldung von Marketo Sales {#marketo-sales-opt-out}

Das Feld Marketo Sales Opt-out ist ein benutzerdefiniertes Feld, das Benutzenden zur Verfügung steht, die das Marketo Sales Insight-Paket ([ AppExchange) ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} haben.

Nachdem Sie das Marketo Sales Insight-Paket erfolgreich von der AppExchange in Salesforce installiert haben, wird das Feld Marketo Sales Opt-Out angezeigt, das Ihnen zur Verfügung steht.
