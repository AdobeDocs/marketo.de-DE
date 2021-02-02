---
unique-page-id: 3571807
description: Schritt 2 von 3 - Einrichten von MarketingTo Sync User in Dynamics (On-Premises 2011) - MarketingTo Docs - Produktdokumentation
title: Schritt 2 von 3 - Einrichten von Marketo Sync User in Dynamics (On-Premises 2011)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Schritt 2 von 3: Einrichten von Marketo Sync User in Dynamics (On-Premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Gute Arbeit, die vorherigen Schritte zu vollenden, lassen Sie uns fortfahren.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren Sie die Marketing Solution (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Synchronisierte Benutzerrolle zuweisen {#assign-sync-user-role}

Weisen Sie die Rolle &quot;Benutzer synchronisieren&quot;nur dem Synchronisierungsbenutzer von Marketing zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für das Marketo-Zusatzmodul Version 4.0.0.14 und höher. Bei älteren Versionen müssen alle Benutzer die Rolle &quot;Synchronisierungsbenutzer&quot;haben. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketing-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Wählen Sie im Menü unten links **Einstellungen**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Wählen Sie in der Struktur **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Wählen Sie **Benutzer**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Hier sehen Sie eine Liste von Benutzern. Wählen Sie Ihren dedizierten Marketo-Synchronisierungsbenutzer oder wenden Sie sich an Ihren [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)-Administrator, um einen neuen Benutzer zu erstellen, der Marketo gewidmet ist. Klicken Sie auf **Rollen verwalten**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Markieren Sie **Markieren Sie den Benutzer** und klicken Sie auf **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM-System vorgenommen hat, werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren von Marketing Solution {#configure-marketo-solution}

Fast fertig! Wir haben nur ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel gehen.

1. Wählen Sie **Einstellungen**. Wählen Sie dann **Marketo Config** in der Struktur.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketing-Lösung erneut](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **Default**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Klicken Sie auf ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Wählen Sie im Popup den Synchronisierungsbenutzer aus. Klicken Sie dann auf **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Klicken Sie auf **Speichern**, um die Änderungen zu speichern.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie zu Schritt 3 fortfahren, {#before-proceeding-to-step}

    * Wenn Sie die Anzahl der synchronisierten Datensätze einschränken möchten, [richten Sie jetzt einen benutzerdefinierten Synchronisierungsfilter ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Führen Sie den Vorgang &quot;[Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)&quot;aus. Es wird überprüft, ob die ersten Setups ordnungsgemäß durchgeführt wurden.
    * Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

Gute Arbeit!

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
