---
description: Hinzufügen von Sales Insight-Zugriff zu Profilen - Marketo Docs - Produktdokumentation
title: Hinzufügen von Sales Insight-Zugriff zu Profilen
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 3%

---

# Hinzufügen von Sales Insight-Zugriff zu Profilen {#add-sales-insight-access-to-profiles}

Hier erfahren Sie, wie Sie ein Profil mit Zugriff auf Sales Insight erstellen und gleichzeitig den Zugriff für Ihre anderen Profile entfernen. Dies ist für Benutzer bestimmt, die bereits das AppExchange-Paket [Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} installiert haben.

>[!IMPORTANT]
>
>Wenn Sie bereits zuvor Sales Insight Zugriff auf alle Profile gewährt haben, müssen Sie [Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}, um diesen Berechtigungssatz zu verwenden.

## Erstellen eines neuen Profils für Sales Insight {#create-a-new-profile-for-sales-insight}

Wenn Sie über ein dediziertes Profil für Ihre Sales Insight-Benutzer verfügen, können Sie diesen Schritt überspringen.

1. Gehen Sie in Salesforce zur Seite Einrichtung .

1. Suchen Sie in der Schnellsuche nach Profilen und wählen Sie die Option **Profil** aus.

1. Klicken Sie oben auf der Seite auf die Schaltfläche **Neues Profil** .

1. Wählen Sie ein zu klonendes Profil aus und geben Sie ihm einen Namen (z. B. Sales Insight User).

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

## Hinzufügen von Sales Insight-Berechtigungen {#add-sales-insight-permissions}

1. Gehen Sie zurück zur Profilliste.

1. Klicken Sie auf den Link **Bearbeiten** für das neue Profil, das Sie gerade erstellt haben (oder ein anderes vorhandenes Profil, auf das Sie Sales Insight zugreifen möchten).

1. Auf der Bearbeitungsseite müssen Sie einige Einstellungen ändern.

   **Für Profile, die auf Sales Insight zugreifen dürfen**:

   * Ändern Sie in den Registerkarteneinstellungen die Marketo-Registerkarten in &quot;Standard ein&quot;
   * Aktivieren Sie unter Benutzerdefinierte Objektberechtigungen die Option Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration (falls der Benutzer Zugriff auf die Konfigurationseinstellungen haben sollte, die normalerweise für Administratoren verwendet werden).

   **Für Profile, die keinen Zugriff auf Sales Insight** haben:

   * Ändern Sie in den Registerkarteneinstellungen die Registerkarten Marketo in Ausgeblendete Registerkarte .
   * Deaktivieren Sie in den Berechtigungen für benutzerdefinierte Objekte die Option Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration.

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

## Erstellen eines Layouts für Sales Insight {#create-layout-for-sales-insight}

1. Gehen Sie zur Seite &quot;Einrichtung&quot;und klicken Sie auf **App-Einrichtung** > **Benutzerspezifisch** > **Leads** > **Seitenlayouts**. Klicken Sie dann auf die Schaltfläche **Neu** .

1. Klonen Sie Ihr Layout Ihrer Wahl und geben Sie dem Layout einen geeigneten Namen (z. B.: Sales Insight Layout).

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Profil dem Layout zuweisen {#assign-profile-to-layout}

1. Gehen Sie zurück zum Abschnitt Seitenlayouts und klicken Sie auf die Schaltfläche **Zuweisen des Seitenlayouts** .

1. Wählen Sie **Zuweisung bearbeiten** aus.

1. Wählen Sie Ihr Sales Insight-Profil aus der Liste und dann Ihr Sales Insight-Layout aus der Dropdown-Liste &quot;Seitenlayout auswählen&quot;.

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Sonstige Änderungen {#other-changes}

Im Folgenden finden Sie einige weitere Stellen, an denen Artikel aus Sales Insight angezeigt werden könnten. Sie müssen sie vollständig entfernen, da Sie Profile nicht verwenden können, um ihren Zugriff zu beschränken:

* Entfernen der Schaltflächen &quot;Sales Insight&quot;aus Suchlayouts für Kontakte, Leads und Konten
* Entfernen von Spalten &quot;Sales Insight&quot;aus Kontakt- und Lead-Listen
