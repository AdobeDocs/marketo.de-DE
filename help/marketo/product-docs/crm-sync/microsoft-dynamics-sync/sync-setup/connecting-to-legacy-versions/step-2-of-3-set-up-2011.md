---
unique-page-id: 3571807
description: 'Schritt 2 von 3: Einrichten des Marketo Sync User in Dynamics (On-Premises 2011) - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Einrichten des Marketo Sync User in Dynamics (On-Premises 2011)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Schritt 2 von 3: Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (On-Premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Gute Arbeit, die vorherigen Schritte abzuschließen, lassen Sie uns weiter durchgehen.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren Sie die Marketo-Lösung (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für das Marketo-Plug-in Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch eingestellt sein](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Wählen Sie im Menü unten links die Option **Einstellungen**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Wählen Sie im Baum **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Auswählen **Benutzer**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Hier sehen Sie eine Liste der Benutzer. Wählen Sie den dedizierten Marketo-Synchronisierungsbenutzer aus oder kontaktieren Sie Ihren [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Administrator , um einen neuen Benutzer zu erstellen, der Marketo gewidmet ist. Klicken **Rollen verwalten**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Überprüfen **Marketo Sync User** und klicken Sie auf **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **not** wieder mit Marketo synchronisiert werden.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast fertig! Wir haben nur einige letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Auswählen **Einstellungen**. Wählen Sie anschließend **Marketo-Konfiguration** im Baum.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, [Marketo-Lösung erneut veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install.md) oder melden Sie sich ab und wieder an.

1. Klicken **Standard**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Klicken Sie auf ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Wählen Sie im Popup-Fenster den Synchronisierungsbenutzer aus. Klicken Sie anschließend auf **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Klicken **Speichern** , um die Änderungen zu speichern.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Klicken **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

    * Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, [richten Sie jetzt einen benutzerdefinierten Synchronisierungsfilter ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Führen Sie den Prozess [Microsoft Dynamics Sync überprüfen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
    * Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

Großartig gemacht!

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect.md)
