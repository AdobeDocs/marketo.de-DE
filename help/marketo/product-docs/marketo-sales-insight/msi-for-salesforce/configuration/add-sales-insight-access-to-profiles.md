---
description: Zugriff von Insight auf Profile hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen des Zugriffs auf Sales Insight für Profile
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 5%

---

# [!DNL Sales Insight] Zugriff auf Profile hinzufügen {#add-sales-insight-access-to-profiles}

Im Folgenden wird beschrieben, wie Sie ein Profil mit Zugriff auf [!DNL Sales Insight] erstellen und dabei den Zugriff für Ihre anderen Profile entfernen. Dies ist für Benutzende gedacht, die das [[!DNL Sales Insight] AppExchange-Paket bereits installiert &#x200B;](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Wenn Sie zuvor [!DNL Sales Insight] Zugriff auf alle Profile gewährt haben, müssen Sie [Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} um diesen Berechtigungssatz zu verwenden.

## Neues Profil für [!DNL Sales Insight] erstellen {#create-a-new-profile-for-sales-insight}

Wenn Sie über ein dediziertes Profil für Ihre [!DNL Sales Insight] Benutzer verfügen, können Sie diesen Schritt überspringen.

1. Navigieren Sie [!DNL Salesforce] zur Seite „Setup“.

1. Suchen Sie in der Schnellsuche nach Profilen und wählen Sie die Option **[!UICONTROL Profil]** aus.

1. Klicken Sie auf **[!UICONTROL Schaltfläche]** Neues Profil“ oben auf der Seite.

1. Wählen Sie ein zu klonendes Profil aus und geben Sie ihm einen Namen (z. B.: Sales Insight User).

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

## [!DNL Sales Insight] hinzufügen {#add-sales-insight-permissions}

1. Kehren Sie zu Ihrer Profilliste zurück.

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**-Link für das neue Profil, das Sie gerade erstellt haben (oder für ein anderes vorhandenes Profil, dem Sie [!DNL Sales Insight] Zugriff gewähren möchten).

1. Auf der Seite „Bearbeiten“ müssen Sie einige Einstellungen ändern.

   **Für Profile mit[!DNL Sales Insight]** Zugriffsberechtigung:

   * Ändern Sie unter „Registerkarteneinstellungen“ die Registerkarten &quot;Marketo&quot; in „Standard ein“
   * Aktivieren Sie unter Benutzerdefinierte Objektberechtigungen die Optionen Lesen, Erstellen, Bearbeiten und Löschen in [!DNL Marketo Sales Insight] Konfiguration (wenn die Benutzenden Zugriff auf die Konfigurationseinstellungen haben sollen, die normalerweise für Admins verwendet werden)

   **Für Profile, für die der Zugriff auf[!DNL Sales Insight]** nicht zulässig ist:

   * Ändern Sie in den Registerkarteneinstellungen die Marketo-Registerkarten in „Registerkarte ausgeblendet“
   * Deaktivieren Sie in Benutzerdefinierte Objektberechtigungen die Optionen Lesen, Erstellen, Bearbeiten und Löschen in [!DNL Marketo Sales Insight] Konfiguration

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

## Layout für [!DNL Sales Insight] erstellen {#create-layout-for-sales-insight}

1. Gehen Sie zur Seite „Einstellungen“ und klicken Sie dann auf **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Anpassen]** > **[!UICONTROL Leads]** > **[!UICONTROL Seitenlayouts]**. Klicken Sie dann auf **[!UICONTROL Neu]**.

1. Klonen Sie Ihr Layout Ihrer Wahl und geben Sie dem Layout einen entsprechenden Namen (z. B.: Sales Insight Layout).

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für Ihre Seitenlayouts [!UICONTROL Kontakte], [!UICONTROL Chancen] und [!UICONTROL Konten].

## Zuweisen eines Profils zum Layout {#assign-profile-to-layout}

1. Gehen Sie zurück zum Abschnitt Seitenlayouts und klicken Sie auf die Schaltfläche **[!UICONTROL Seitenlayoutzuweisung]**.

1. Wählen Sie **[!UICONTROL Zuweisung bearbeiten]** aus.

1. Wählen Sie Ihr [!DNL Sales Insight] aus der Liste und dann Ihr [!DNL Sales insight] Layout aus der Dropdown-Liste [!UICONTROL Auswählen &#x200B;]Seitenlayouts“ aus.

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

1. Wiederholen Sie diese Schritte für Ihre Seitenlayouts [!UICONTROL Kontakte], [!UICONTROL Chancen] und [!UICONTROL Konten].

## Sonstige Änderungen {#other-changes}

Hier sind einige andere Stellen, an denen [!DNL Sales Insight] Elemente angezeigt werden könnten. Sie müssen sie vollständig entfernen, da Sie Profile nicht verwenden können, um ihren Zugriff zu beschränken:

* Entfernen Sie [!DNL Sales Insight] Schaltflächen aus den Suchlayouts [!UICONTROL Kontakte], [!UICONTROL Leads] und [!UICONTROL Konten]
* [!DNL Sales Insight] Spalten aus Kontakt- und Lead-Listen entfernen
