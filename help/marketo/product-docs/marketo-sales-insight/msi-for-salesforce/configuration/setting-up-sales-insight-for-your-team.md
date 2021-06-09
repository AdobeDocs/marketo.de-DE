---
description: Einrichten von Sales Insight für Ihr Team - Marketo Docs - Produktdokumentation
title: Einrichten von Sales Insight für Ihr Team
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Einrichten von Sales Insight für Ihr Team {#setting-up-sales-insight-for-your-team}

Hier erfahren Sie, wie Sie ein Profil mit Zugriff auf Sales Insight erstellen und gleichzeitig den Zugriff für Ihre anderen Profile entfernen. Dies ist für Benutzer bestimmt, die das [Sales Insight-AppExchange-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) bereits installiert haben.

## Erstellen eines neuen Profils für Sales Insight {#create-a-new-profile-for-sales-insight}

Wenn Sie über ein dediziertes Profil für Ihre Sales Insight-Benutzer verfügen, können Sie diesen Schritt überspringen.

1. Gehen Sie in Salesforce zur Seite Einrichtung .

1. Suchen Sie in der Schnellsuche nach Profilen und wählen Sie die Option **Profil** aus.

1. Klicken Sie oben auf der Seite auf die Schaltfläche **Neues Profil** .

1. Wählen Sie ein zu klonendes Profil aus und geben Sie ihm einen Namen (z. B.: Sales Insight-Benutzer).

1. Klicken Sie abschließend auf **Speichern** .

## Hinzufügen von Sales Insight-Berechtigungen {#add-sales-insight-permissions}

1. Gehen Sie zurück zur Profilliste.

1. Klicken Sie auf den Link **Bearbeiten** für das neue Profil, das Sie gerade erstellt haben (oder ein anderes vorhandenes Profil, dem Sie Sales Insight-Zugriff gewähren möchten).

1. Auf der Bearbeitungsseite müssen Sie einige Einstellungen ändern.

   **Für Profile, die Zugriff auf Sales Insight haben**:

   * Ändern Sie in den Registerkarteneinstellungen die Marketo-Registerkarten in &quot;Standard ein&quot;
   * Aktivieren Sie unter Benutzerdefinierte Objektberechtigungen die Option Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration (falls der Benutzer Zugriff auf die Konfigurationseinstellungen haben sollte, die normalerweise für Administratoren verwendet werden).

   **Für Profile, die keinen Zugriff auf Sales Insight** haben:

   * Ändern Sie in den Registerkarteneinstellungen die Registerkarten Marketo in Ausgeblendete Registerkarte .
   * Deaktivieren Sie in den Berechtigungen für benutzerdefinierte Objekte die Option Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration.


1. Klicken Sie abschließend auf **Speichern** .

## Layout für Sales Insight erstellen {#create-layout-for-sales-insight}

1. Gehen Sie zur Seite &quot;Einrichtung&quot;und klicken Sie auf **App-Einrichtung** > **Anpassen** > **Leads** > **Seitenlayouts**. Klicken Sie dann auf die Schaltfläche **Neu**.

1. Klonen Sie das Layout Ihrer Wahl und geben Sie dem Layout einen geeigneten Namen (z. B.: Sales Insight-Layout).

1. Klicken Sie abschließend auf **Speichern** .

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Profil dem Layout zuweisen {#assign-profile-to-layout}

1. Gehen Sie zurück zum Abschnitt Seitenlayouts und klicken Sie auf die Schaltfläche **Seitenlayoutzuweisung** .

1. Wählen Sie **Zuweisung bearbeiten**.

1. Wählen Sie Ihr Sales Insight-Profil aus der Liste und dann Ihr Sales Insight-Layout aus der Dropdown-Liste &quot;Seitenlayout auswählen&quot;.

1. Klicken Sie abschließend auf **Speichern** .

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Sonstige Änderungen {#other-changes}

Im Folgenden finden Sie einige weitere Stellen, an denen Artikel aus Sales Insight angezeigt werden könnten. Sie müssen sie vollständig entfernen, da Sie Profile nicht verwenden können, um ihren Zugriff zu beschränken:

* Entfernen der Schaltflächen &quot;Sales Insight&quot;aus &quot;Suchlayouts für Kontakte, Leads und Konten&quot;
* Entfernen von Spalten &quot;Sales Insight&quot;aus Kontakt- und Lead-Listen
