---
unique-page-id: 7504739
description: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3 - Marketing Docs - Produktdokumentation
title: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Schritt 2 von 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

Gute Arbeit beim Abschluss der vorherigen Schritte. Lasst uns das weitermachen.

>[!PREREQUISITES]
>
>* [Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3](step-1-of-3-install.md)

>



## Synchronisierte Benutzerrolle zuweisen {#assign-sync-user-role}

Weisen Sie die Rolle &quot;Benutzer synchronisieren&quot;nur dem Synchronisierungsbenutzer von Marketing zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für Marketo Version 4.0.0.14 und höher. Bei älteren Versionen müssen alle Benutzer die Rolle &quot;Synchronisierungsbenutzer&quot;haben. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketing-Lösung für Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

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
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM-System vorgenommen hat, werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren von Marketing Solution {#configure-marketo-solution}

Fast fertig! Wir haben nur ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel gehen.

1. Klicken Sie unter **Einstellungen** auf **Marketing-Konfiguration**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, veröffentlichen Sie [die Marketing-Lösung](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) oder versuchen Sie, sich abzumelden und wieder anzumelden.

1. Klicken Sie auf **Default**.

   ![](assets/configure2.png)

1. Klicken Sie auf das Feld **Markieren Sie den Benutzer** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/configure3.png)

1. Klicken Sie auf das Symbol Speichern in der unteren rechten Ecke.

   ![](assets/configure4.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie zu Schritt 3 fortfahren, {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze einschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ein.
* Führen Sie den Prozess [Microsoft Dynamics Sync ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) überprüfen aus. Es wird überprüft, ob die ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3](step-3-of-3-connect.md)
