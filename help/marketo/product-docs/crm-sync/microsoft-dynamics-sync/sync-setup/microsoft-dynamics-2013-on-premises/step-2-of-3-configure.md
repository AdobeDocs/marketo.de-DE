---
unique-page-id: 3571816
description: 'Schritt 2 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013) - Marketo Docs - Produktdokumentation'
title: Schritt 2 von 3 - Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Schritt 2 von 3: Konfigurieren von Synchronisierungsbenutzer für Marketo (On-Premises 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Gute Arbeit, die vorherigen Schritte abzuschließen, lassen Sie uns weiter durchgehen.

>[!PREREQUISITES]
[Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)>
>

## Benutzerrolle &quot;Sync zuweisen&quot;{#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
Dies gilt für das Marketo-Plug-in Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf &quot;English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)&quot;gesetzt werden.

1. Klicken Sie unter **Settings** auf **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Wählen Sie **Benutzer** aus.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Hier sehen Sie eine Liste der Benutzer. Wählen Sie Ihren dedizierten Marketo-Synchronisierungsbenutzer aus oder kontaktieren Sie Ihren [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [Administrator, um einen neuen Marketo-spezifischen Benutzer zu erstellen.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie auf ![](assets/image2015-3-26-11-3a16-3a22.png) und wählen Sie **Rollen verwalten** aus.

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Markieren Sie **Marketo Sync User** und klicken Sie auf **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast fertig! Wir haben nur einige letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Klicken Sie unter **Settings** auf **Marketo Config**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   Wenn **Marketo Config** fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketo-Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) erneut oder versuchen Sie, sich ab- und wieder anzumelden.

1. Klicken Sie auf **Default**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicken Sie auf das Feld **Marketo User** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicken Sie unten rechts auf ![](assets/image2015-3-13-15-3a10-3a11.png) , um die Änderungen zu speichern.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ein.
* Führen Sie den Prozess [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) überprüfen aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

Großartig gemacht!

>[!MORELIKETHIS]
[Schritt 3 von 3: Marketo und Dynamics verbinden (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
