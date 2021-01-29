---
unique-page-id: 3571816
description: Schritt 2 von 3 - Konfigurieren des Synchronisierungsbenutzers für Marketing (On-Premises 2013) - Marketing Docs - Produktdokumentation
title: Schritt 2 von 3 - Konfigurieren des Synchronisierungsbenutzers für Marketing (On-Premises 2013)
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Schritt 2 von 3: Konfigurieren des Synchronisierungsbenutzers für Marketo (On-Premises 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Gute Arbeit, die vorherigen Schritte zu vollenden, lassen Sie uns fortfahren.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren Sie die Marketing Solution in Dynamics (On-Premises 2013)](step-1-of-3-install.md)


## Synchronisierte Benutzerrolle zuweisen {#assign-sync-user-role}

Weisen Sie die Rolle &quot;Benutzer synchronisieren&quot;nur dem Synchronisierungsbenutzer von Marketing zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für das Marketo-Zusatzmodul Version 4.0.0.14 und höher. Bei älteren Versionen müssen alle Benutzer die Rolle &quot;Synchronisierungsbenutzer&quot;haben. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketing-Lösung für Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Klicken Sie unter **Einstellungen** auf **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Wählen Sie **Benutzer**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Hier sehen Sie eine Liste von Benutzern. Wählen Sie Ihren dedizierten Marketo-Sync-Benutzer oder wenden Sie sich an Ihren [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [Administrator, um einen neuen Benutzer zu erstellen, der Marketo gewidmet ist.](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie auf ![](assets/image2015-3-26-11-3a16-3a22.png)und wählen Sie **Rollen verwalten**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Markieren Sie **Markieren Sie den Benutzer** und klicken Sie auf **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM-System vorgenommen hat, werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren von Marketing Solution {#configure-marketo-solution}

Fast fertig! Wir haben nur ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel gehen.

1. Klicken Sie unter **Einstellungen** auf **Marketing-Konfiguration**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Wenn **Marketo-Konfiguration** fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketing-Lösung](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) erneut oder versuchen Sie, sich abzumelden und wieder einzuloggen.

1. Klicken Sie auf **Default**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicken Sie auf das Feld **Markieren Sie den Benutzer** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicken Sie in der unteren rechten Ecke auf ![](assets/image2015-3-13-15-3a10-3a11.png), um die Änderungen zu speichern.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie zu Schritt 3 fortfahren, {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze einschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ein.
* Führen Sie den Prozess [Microsoft Dynamics Sync ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) überprüfen aus. Es wird überprüft, ob die ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

Gute Arbeit!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Schritt 3 von 3: Connect Marketing and Dynamics (On-Premises 2013)](step-3-of-3-connect.md)

