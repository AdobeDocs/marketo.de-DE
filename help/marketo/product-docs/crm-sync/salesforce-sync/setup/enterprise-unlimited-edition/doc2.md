---
description: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited) - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)'
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 2%

---

# Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator durchgeführt werden

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

In diesem Artikel richten Sie Benutzerberechtigungen im Salesforce-Profil ein und erstellen ein Marketo-Salesforce-Integrationskonto.

## Profil erstellen {#create-a-profile}

1. Klicken Sie **[!UICONTROL Setup]**.

   SCREENSHOT

1. Geben Sie „Profile“ in die Navigationssuchleiste ein und klicken Sie auf den Link Profile .

   SCREENSHOT

1. Klicken Sie auf Neues Profil.

   SCREENSHOT

1. Wählen Sie Standardbenutzer, benennen Sie das Profil &quot;Marketo-Salesforce Sync“ und klicken Sie auf Speichern.

   SCREENSHOT

## Festlegen von Profilberechtigungen {#set-profile-permissions}

1. Klicken Sie auf Bearbeiten , um die Sicherheitsberechtigungen festzulegen.

   SCREENSHOT

1. Stellen Sie im Abschnitt Administratorberechtigungen sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * API-fähig
   * HTML-Vorlagen bearbeiten
   * Öffentliche Dokumente verwalten
   * Verwalten öffentlicher Vorlagen

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie das Kontrollkästchen „Kennwort läuft nie ab“ aktivieren.

1. Stellen Sie im Abschnitt Allgemeine Benutzerberechtigungen sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * Leads konvertieren
   * Ereignisse bearbeiten
   * Aufgaben bearbeiten

1. Stellen Sie im Abschnitt Standardobjektberechtigungen sicher, dass die Berechtigungen Lesen, Erstellen, Bearbeiten und Löschen für Folgendes aktiviert sind:

   * Konten
   * Kampagnen
   * Kontakte
   * Leads
   * Opportunitys

   >[!NOTE]
   >
   >Gewähren Sie den Kampagnen Berechtigungen, wenn Sie die Kampagnensynchronisierung verwenden möchten.

   SCREENSHOT

1. Klicken Sie abschließend unten auf der Seite auf Speichern .

   SCREENSHOT

## Festlegen von Feldberechtigungen {#set-field-permissions}

1. Besprechen Sie mit Ihren Marketern, um herauszufinden, welche benutzerdefinierten Felder zum Synchronisieren erforderlich sind.

   >[!NOTE]
   >
   >Dieser Schritt verhindert, dass Felder, die Sie nicht benötigen, in Marketo angezeigt werden. Dadurch wird die Anzeige übersichtlicher und die Synchronisierung beschleunigt.

1. Gehen Sie auf der Seite mit den Profildetails zum Abschnitt Sicherheit auf Feldebene . Klicken Sie auf Ansicht , um die Barrierefreiheit für die Objekte zu bearbeiten:

   * Lead
   * Kontakt
   * Konto
   * Opportunity

   >[!TIP]
   >
   >Sie können andere Objekte entsprechend den Anforderungen Ihres Unternehmens konfigurieren.

1. Klicken Sie für jedes Objekt auf Bearbeiten.

   SCREENSHOT

1. Suchen Sie die nicht benötigten Felder und stellen Sie sicher, dass Lesezugriff und Bearbeitungszugriff deaktiviert sind. Klicken Sie abschließend auf Speichern .

   >[!NOTE]
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

   SCREENSHOT

1. Nachdem Sie alle nicht benötigten Felder deaktiviert haben, müssen Sie Lesezugriff und Bearbeitungszugriff für die folgenden Objektfelder aktivieren. Klicken Sie abschließend auf Speichern .

   TABELLE

   SCREENSHOT

## Synchronisierungskonto für Marketo-Salesforce erstellen {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Erstellen Sie ein dediziertes Salesforce-Konto (z. B. `marketo@yourcompany.com`), um die von Marketo vorgenommenen Änderungen von denen anderer Salesforce-Benutzender zu unterscheiden.

1. Geben Sie in die Navigationssuchleiste „Benutzer verwalten“ ein und klicken Sie dann auf Benutzer . Klicken Sie auf Neuer Benutzer.

   SCREENSHOT

   SCREENSHOT

1. Füllen Sie die erforderlichen Felder aus. Wählen Sie dann die Benutzerlizenz: Salesforce und das zuvor erstellte Profil aus. Klicken Sie abschließend auf Speichern .

   SCREENSHOT

Schritt 2 von 3 ist abgeschlossen.
