---
unique-page-id: 7504739
description: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3 - Marketing Docs - Produktdokumentation
title: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Schritt 2 von 3 Einrichten von Marketing for Dynamics (On-Prem 2015 und On-Prem 2016 365){#step-of-set-up-for-marketo-on-premises-and-365}

Gute Arbeit beim Abschluss der vorherigen Schritte. Lasst uns das weitermachen.

>[!PREREQUISITES]
>
>[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Synchronisierte Benutzerrolle zuweisen {#assign-sync-user-role}

Weisen Sie die Rolle &quot;Benutzer synchronisieren&quot;nur dem Synchronisierungsbenutzer von Marketing zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für Marketo Version 4.0.0.14 und höher. Bei älteren Versionen müssen alle Benutzer die Rolle &quot;Synchronisierungsbenutzer&quot;haben. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketing-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Klicken Sie unter **Einstellungen** auf **Sicherheit**.

   ![](assets/assign1.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/assign2.png)

1. Hier sehen Sie eine Liste von Benutzern. Wählen Sie den dedizierten Marketo-Sync-Benutzer oder wenden Sie sich an Ihren [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)-Administrator, um einen dedizierten Benutzer für Marketo zu erstellen.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie auf **Rollen verwalten**.

   ![](assets/assign4.png)

   Markieren Sie &quot;Benutzer synchronisieren&quot;und klicken Sie auf &quot;OK&quot;.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM-System vorgenommen hat, werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren von Marketing Solution {#configure-marketo-solution}

Fast fertig! Wir haben nur ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel gehen.

1. Klicken Sie unter **Einstellungen** auf **Marketing-Konfiguration**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketing-Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) oder versuchen Sie, sich abzumelden und wieder anzumelden.

1. Klicken Sie auf **Default**.

   ![](assets/configure2.png)

1. Klicken Sie auf das Feld **Markieren Sie den Benutzer** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/configure3.png)

1. Klicken Sie auf das Symbol Speichern in der unteren rechten Ecke.

   ![](assets/configure4.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie zu Schritt 3 fortfahren, {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze einschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ein.
* Führen Sie den Prozess [Microsoft Dynamics Sync ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) überprüfen aus. Es wird überprüft, ob die ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
>
>[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
