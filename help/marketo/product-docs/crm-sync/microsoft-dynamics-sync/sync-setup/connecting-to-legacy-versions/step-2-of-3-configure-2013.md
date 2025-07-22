---
unique-page-id: 3571816
description: Schritt 2 von 3 - Synchronisierungsbenutzer für Marketo konfigurieren (2013 On-Premise) - Marketo-Dokumente - Produktdokumentation
title: Schritt 2 von 3 - Synchronisierungsbenutzer für Marketo konfigurieren (2013 On-Premise)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Schritt 2 von 3: Synchronisierungsbenutzer für Marketo konfigurieren (2013 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises}

Gute Arbeit beim Abschließen der vorherigen Schritte, lassen Sie uns dies weiter durchgehen.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketo-Lösung in  [!DNL Dynamics] (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)

## Assign Sync User Role {#assign-sync-user-role}

Weisen Sie die Rolle Marketo-Synchronisierungsbenutzer nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Plug-in-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Rolle „Benutzer synchronisieren“ verfügen. Informationen zum Upgrade von Marketo finden Sie [Upgrade der Marketo-Lösung für [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch festgelegt werden](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Administration]**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Wählen Sie **[!UICONTROL Benutzer]** aus.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Hier wird eine Liste der Benutzer angezeigt. Wählen Sie Ihren dedizierten Marketo Sync-Benutzer aus oder wenden Sie sich an Ihren [Active Directory Federation Services (AFDS](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"}-Administrator, um einen neuen Benutzer zu erstellen, der [dediziert für Marketo](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx){target="_blank"} ist.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie auf ![](assets/image2015-3-26-11-3a16-3a22.png) und wählen Sie **[!UICONTROL Rollen verwalten]**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Markieren Sie **[!UICONTROL Marketo-Synchronisierungsbenutzer]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Wenn Sie die Rolle nicht sehen, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"} und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM vorgenommen hat, _nicht_ wieder mit Marketo synchronisiert.

## Marketo-Lösung konfigurieren {#configure-marketo-solution}

Fast fertig! Wir haben nur noch ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Marketo Config]**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Wenn **[!UICONTROL Marketo Config]** fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht[ veröffentlichen Sie die Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)Lösung erneut oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicken Sie auf das Feld **[!UICONTROL Marketo-Benutzer]** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicken Sie auf ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicken Sie **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, richten [ jetzt einen benutzerdefinierten Synchronisierungsfilter ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Führen Sie den Prozess [validate [!DNL Microsoft Dynamics] sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es stellt sicher, dass die anfänglichen Setups korrekt ausgeführt wurden.
* Melden Sie sich beim Marketo Sync User in [!DNL Microsoft Dynamics] CRM an.

Großartig gemacht!

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Marketo verbinden und [!DNL Dynamics] (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md)
