---
unique-page-id: 7504739
description: Installieren Sie Marketo für Dynamics 2015 On-Premise und 2016 On-Premise 365 (On-Premise-Schritt 2 von 3 - Marketo Docs - Produktdokumentation
title: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Schritt 2 von 3 Marketo für Dynamics einrichten (On-Premise 2015 und On-Premise 2016 365){#step-of-set-up-for-marketo-on-premises-and-365}

Große Arbeit zum Abschluss der vorherigen Schritte. Lasst uns das durchgehen.

>[!PREREQUISITES]
[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)>
>

## Benutzerrolle &quot;Sync zuweisen&quot;{#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren Ihres Marketo finden Sie unter [Aktualisieren der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf &quot;English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)&quot;gesetzt werden.

1. Klicken Sie unter **Settings** auf **Security**.

   ![](assets/assign1.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/assign2.png)

1. Hier sehen Sie eine Liste der Benutzer. Wählen Sie den dedizierten Marketo Sync-Benutzer aus oder kontaktieren Sie Ihren Administrator [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) , um einen dedizierten Benutzer für Marketo zu erstellen.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie auf **Rollen verwalten**.

   ![](assets/assign4.png)

   Markieren Sie Marketo Sync User und klicken Sie auf OK.

   ![](assets/assign5.png)

   >[!TIP]
   Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast fertig! Wir haben nur einige letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Klicken Sie unter **Settings** auf **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketo-Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) oder versuchen Sie, sich ab- und wieder anzumelden.

1. Klicken Sie auf **Default**.

   ![](assets/configure2.png)

1. Klicken Sie auf das Feld **Marketo User** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/configure3.png)

1. Klicken Sie unten rechts auf das Symbol Speichern .

   ![](assets/configure4.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ein.
* Führen Sie den Prozess [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) überprüfen aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
