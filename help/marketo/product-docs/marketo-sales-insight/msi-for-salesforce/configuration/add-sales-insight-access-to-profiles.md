---
description: Hinzufügen von Sales Insights-Zugriff zu Profilen - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von Sales Insights-Zugriff zu Profilen
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 3%

---

# Hinzufügen von Sales Insights-Zugriff zu Profilen {#add-sales-insight-access-to-profiles}

Im Folgenden wird beschrieben, wie Sie ein Profil mit Zugriff auf Sales Insight erstellen und dabei den Zugriff für Ihre anderen Profile entfernen. Dies ist für Benutzende gedacht, die bereits das [Sales Insight AppExchange-Paket“ installiert ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Wenn Sie zuvor Sales Insights Zugriff auf alle Profile gewährt haben, müssen Sie [Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} um diesen Berechtigungssatz zu verwenden.

## Erstellen eines neuen Profils für Sales Insight {#create-a-new-profile-for-sales-insight}

Wenn Sie über ein dediziertes Profil für Ihre Sales Insight-Benutzer verfügen, können Sie diesen Schritt überspringen.

1. Navigieren Sie in Salesforce zur Seite „Setup“.

1. Suchen Sie in der Schnellsuche nach Profilen und wählen Sie die Option **Profil** aus.

1. Klicken Sie auf **Schaltfläche** Neues Profil“ oben auf der Seite.

1. Wählen Sie ein zu klonendes Profil aus und geben Sie ihm einen Namen (z. B.: Sales Insight-Benutzer).

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

## Hinzufügen von Berechtigungen für Sales Insights {#add-sales-insight-permissions}

1. Kehren Sie zu Ihrer Profilliste zurück.

1. Klicken Sie auf **Bearbeiten**-Link für das neue Profil, das Sie gerade erstellt haben (oder für ein anderes vorhandenes Profil, dem Sie Sales Insights Zugriff gewähren möchten).

1. Auf der Seite „Bearbeiten“ müssen Sie einige Einstellungen ändern.

   **Für Profile mit Zugriffsberechtigung auf Sales Insight**:

   * Ändern Sie unter „Registerkarteneinstellungen“ die Registerkarten &quot;Marketo&quot; in „Standard ein“
   * Aktivieren Sie unter „Benutzerdefinierte Objektberechtigungen“ die Option Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration (wenn die Benutzenden Zugriff auf die Konfigurationseinstellungen haben sollen, die normalerweise für Admins verwendet werden)

   **Für Profile, denen der Zugriff auf Sales Insight nicht erlaubt ist**:

   * Ändern Sie in den Registerkarteneinstellungen die Marketo-Registerkarten in „Registerkarte ausgeblendet“
   * Deaktivieren Sie in Benutzerdefinierte Objektberechtigungen Lesen, Erstellen, Bearbeiten und Löschen in der Marketo Sales Insight-Konfiguration

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

## Erstellen eines Layouts für Sales Insight {#create-layout-for-sales-insight}

1. Gehen Sie zur Seite „Einstellungen“ und klicken Sie dann auf **Anwendungseinstellungen** > **Anpassen** > **Leads** > **Seitenlayouts**. Klicken Sie dann auf **Neu**.

1. Klonen Sie Ihr Layout Ihrer Wahl und geben Sie dem Layout einen entsprechenden Namen (z. B.: Sales Insight Layout).

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für die Seiten-Layouts Ihrer Kontakte, Vertriebschancen und Konten.

## Zuweisen eines Profils zum Layout {#assign-profile-to-layout}

1. Gehen Sie zurück zum Abschnitt Seitenlayouts und klicken Sie auf die Schaltfläche **Seitenlayoutzuweisung**.

1. Wählen Sie **Zuweisung bearbeiten** aus.

1. Wählen Sie Ihr Sales Insights-Profil aus der Liste und dann Ihr Sales Insights-Layout aus der Dropdown-Liste „Seitenlayout auswählen“ aus.

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für die Seiten-Layouts Ihrer Kontakte, Vertriebschancen und Konten.

## Sonstige Änderungen {#other-changes}

Im Folgenden finden Sie weitere Orte, an denen Sales Insight-Elemente angezeigt werden könnten. Sie müssen sie vollständig entfernen, da Sie Profile nicht verwenden können, um ihren Zugriff zu beschränken:

* Entfernen Sie die Schaltflächen „Sales Insights“ aus den Suchlayouts für Kontakte, Leads und Konten
* Spalten mit Sales Insights aus Kontakt- und Lead-Listen entfernen
