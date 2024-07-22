---
unique-page-id: 14746188
description: Synchronisieren von Abmeldungen mit Salesforce - Marketo Docs - Produktdokumentation
title: Synchronisieren von Abmeldungen mit Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Synchronisieren von Abmeldungen mit Salesforce {#syncing-unsubscribes-with-salesforce}

## Voraussetzungen für Abmeldungen zur Synchronisierung mit Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synchronisierung des Abmeldes muss aktiviert sein (für nächtliche Synchronisation)
* Das Feld Opt-out muss in Salesforce installiert sein.
* Personendatensätze in Sales Connect müssen über eine Salesforce-ID verfügen

**Push unsubscribes**

Wenn eine Abmeldung in Sales Connect erfasst wird, senden wir sie in Echtzeit an Salesforce und aktualisieren eines der Opt-out-Felder, mit denen Sie die Synchronisation ausgewählt haben. Wenn Sie die Salesforce-Synchronisation deaktiviert haben, werden wir die Abmeldung weiterhin an die E-Mail-Abmeldung weiterleiten.

**Synchronisation abmelden**

Wenn Sie die Synchronisation zum Abmelden aktiviert haben (Schritt 3 unten), wird die nächtliche Synchronisation aktiviert. Die Synchronisierung findet einmal täglich um 20:00 Uhr PST statt. Dadurch werden alle Abmeldungen in Marketo Sales bidirektional mit dem Opt-out-Feld in Salesforce synchronisiert.

## Konfigurieren der Abmeldesynchronisierung mit Salesforce {#configure-unsubscribe-sync-to-salesforce}

Benutzer können entscheiden, ob sie ihre Abmeldungen mit dem standardmäßigen Feld für die E-Mail-Abmeldung synchronisieren möchten, mit dem Marketo auch synchronisieren kann, oder sie können mit dem Feld für die Marketo-Abmeldung für Vertrieb synchronisieren, sodass zwischen Abmeldungen für Vertrieb und Abmeldungen für Marketing unterschieden werden kann.

1. Wechseln Sie zur [Webanwendung](https://toutapp.com/login), klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one-1.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Unsubscribes**.

   ![](assets/two-2.png)

1. Klicken Sie auf **Synchronisieren mit Salesforce** und aktivieren Sie dann die nächtliche Synchronisierung.

   ![](assets/three-2.png)

1. Wählen Sie das Feld aus, mit dem Sie synchronisieren möchten.

   ![](assets/4.png)

   | Feld | Beschreibung |
   |---|---|
   | **Mit Salesforce-Opt-out-Feld synchronisieren** | Standardmäßig ausgewählt, wird nur das Feld Salesforce Opt-out aktualisiert. |
   | **Mit Marketo Sales Opt-out-Feld synchronisieren** | Wenn Sie die Abmeldungen für Vertrieb und Marketing trennen möchten, wählen Sie diese Option, um das zusätzliche Feld für die Abmeldung von Marketo-Verkäufen zu aktualisieren.](#msoo)[ |

## Installieren des Felds &quot;Opt-out&quot;im Seitenlayout {#installing-the-opt-out-field-in-the-page-layout}

**E-Mail-Opt-out**

Email Opt-out ist ein Standardfeld in Salesforce, das über Salesforce installiert werden kann. Sie müssen Salesforce-Administrator sein, um es zu installieren.

1. Gehen Sie zu [Salesforce.com](https://salesforce.com) und melden Sie sich an.

   ![](assets/five-1.png)

1. Klicken Sie auf Ihren Benutzernamen und wählen Sie **Einrichten** aus.

   ![](assets/six-1.png)

1. Suchen Sie im Schnellsuchfeld nach Kontakt oder Lead. In diesem Szenario installieren wir das Feld im Layout Kontaktseite , aber Sie sollten es für beide Personendatensätze installieren.

   ![](assets/seven-1.png)

1. Wählen Sie **Seitenlayouts** aus.

   ![](assets/eight-1.png)

1. Wählen Sie neben dem Seitenlayout, dem Sie das Feld hinzufügen möchten, die Option **Bearbeiten** aus.

   ![](assets/nine.png)

1. Wählen Sie **Felder** aus.

   ![](assets/ten.png)

1. Ziehen Sie E-Mail-Opt-out in das Seitenlayout.

   ![](assets/11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/twelve.png)

## Abmeldung von Marketo Sales {#marketo-sales-opt-out}

Das Feld Marketo Sales Opt-out ist ein benutzerdefiniertes Feld, das Benutzern zur Verfügung steht, die die Marketo Sales Connect-Anpassungen installiert haben.

Nachdem Sie die Marketo Sales Connect-Anpassungen erfolgreich in Salesforce installiert haben, sehen Sie das Feld Marketo Sales Opt-out , das Ihnen zur Verfügung steht.
