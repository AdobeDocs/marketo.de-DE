---
description: Einrichten von Sales Insight für Ihr Team - Marketing Docs - Produktdokumentation
title: Einrichten von Sales Insight für Ihr Team
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Einrichten von Sales Insight für Ihr Team {#setting-up-sales-insight-for-your-team}

Im Folgenden wird beschrieben, wie Sie ein Profil mit Zugriff auf Sales Insight erstellen und gleichzeitig den Zugriff auf Ihre anderen Profil entfernen. Dies ist für Benutzer gedacht, die bereits das [Sales Insight-AppExchange-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) installiert haben.

## Neues Profil für Sales Insight {#create-a-new-profile-for-sales-insight} erstellen

Wenn Sie über ein dediziertes Profil für Ihre Sales Insight-Benutzer verfügen, können Sie diesen Schritt überspringen.

1. Gehen Sie in Salesforce zur Seite &quot;Einstellungen&quot;.

1. Suchen Sie in der Schnellsuche nach Profilen und wählen Sie die Option **Profil**.

1. Klicken Sie oben auf der Seite auf die Schaltfläche **Neues Profil**.

1. Wählen Sie ein zu klonendes Profil und geben Sie ihm einen Namen (z. B.: Sales Insight-Benutzer).

1. Klicken Sie abschließend auf **Speichern**.

## hinzufügen Sales Insight-Berechtigungen {#add-sales-insight-permissions}

1. Geh zurück zur Liste deiner Profile.

1. Klicken Sie auf den Link **Bearbeiten** für das neu erstellte Profil (oder ein anderes vorhandenes Profil, auf das Sie Sales Insight zugreifen möchten).

1. Auf der Bearbeitungsseite müssen Sie einige Einstellungen ändern.

   **Für Profil, die Zugriff auf Sales Insight** haben:

   * Aktivieren Sie in den benutzerdefinierten App-Einstellungen die Option &quot;Markieren&quot;, um die Marketing-App sichtbar zu machen.
   * Ändern Sie in den Registerkarteneinstellungen die Registerkarte &quot;Markieren&quot;in &quot;Standard ein&quot;.
   * Aktivieren Sie unter &quot;Benutzerdefinierte Objektberechtigungen&quot;die Optionen &quot;Lesen&quot;, &quot;Erstellen&quot;, &quot;Bearbeiten&quot;und &quot;Löschen&quot;bei &quot;Marketing to Sales Insight Config&quot;(sofern der Benutzer Zugriff auf die Konfigurationseinstellungen haben sollte - die normalerweise für Administratoren verwendet werden).

   **Für Profil, die keinen Zugriff auf Sales Insight** haben:

   * Deaktivieren Sie in den benutzerdefinierten App-Einstellungen die Markierung, um die Marketing-App auszublenden.
   * Ändern Sie in den Registerkarteneinstellungen die Registerkarte &quot;Markieren&quot;in &quot;Tabulator ausgeblendet&quot;.
   * Deaktivieren Sie unter &quot;Benutzerdefinierte Objektberechtigungen&quot;die Optionen &quot;Lesen&quot;, &quot;Erstellen&quot;, &quot;Bearbeiten&quot;und &quot;Löschen&quot;bei &quot;Marketing to Sales Insight Config&quot;.


1. Klicken Sie abschließend auf **Speichern**.

## Layout für Sales Insight erstellen {#create-layout-for-sales-insight}

1. Gehen Sie zur Seite &quot;Einstellungen&quot;und klicken Sie dann auf **App-Einrichtung** > **Anpassen** > **Interessenten** > **Seitenlayouts**. Klicken Sie dann auf die Schaltfläche **Neu**.

1. Klonen Sie das gewünschte Layout und geben Sie dem Layout einen entsprechenden Namen (z. B.: Sales Insight-Layout).

1. Klicken Sie abschließend auf **Speichern**.

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Profil zu Layout {#assign-profile-to-layout} zuweisen

1. Gehen Sie zurück zum Abschnitt &quot;Seitenlayouts&quot;und klicken Sie auf die Schaltfläche **Seitenlayoutzuweisung**.

1. Wählen Sie **Zuweisung bearbeiten**.

1. Wählen Sie Ihr Sales Insight-Profil aus der Liste und wählen Sie dann Ihr Sales Insight-Layout aus der Dropdownliste &quot;Seitenlayout auswählen&quot;.

1. Klicken Sie abschließend auf **Speichern**.

1. Wiederholen Sie diese Schritte für die Seitenlayouts Ihrer Kontakte, Chancen und Konten.

## Andere Änderungen {#other-changes}

Hier sind einige weitere Stellen, an denen Sales Insight-Artikel angezeigt werden können. Sie müssen sie vollständig entfernen, da Sie Profil nicht verwenden können, um ihren Zugriff zu beschränken:

* Entfernen Sie die Schaltflächen &quot;Sales Insight&quot;aus den Layouts für Kontakte, Interessenten und Konten.
* Entfernen Sie die Spalten &quot;Sales Insight&quot;aus den Listen &quot;Kontakt&quot;und &quot;Interessent&quot;.
