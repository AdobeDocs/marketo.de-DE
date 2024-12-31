---
unique-page-id: 3571807
description: Schritt 2 von 3 - Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (2011 On-Premise) - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 2 von 3: Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (2011 On-Premise)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Schritt 2 von 3: Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (2011 On-Premise) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Gute Arbeit beim Abschließen der vorherigen Schritte, lassen Sie uns dies weiter durchgehen.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketo-Lösung (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Assign Sync User Role {#assign-sync-user-role}

Weisen Sie die Rolle Marketo-Synchronisierungsbenutzer nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Plug-in-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Rolle „Benutzer synchronisieren“ verfügen. Informationen zum Upgrade von Marketo finden Sie [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch festgelegt werden](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Wählen Sie im linken unteren Menü die Option **[!UICONTROL Einstellungen]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Wählen Sie in der Struktur **[!UICONTROL Administration]** aus.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Wählen Sie **[!UICONTROL Benutzer]** aus.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Hier wird eine Liste der Benutzer angezeigt. Wählen Sie Ihren dedizierten Marketo-Synchronisierungsbenutzer aus oder wenden Sie sich an Ihren [Active Directory Federation Services (AFDS](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"}-Administrator, um einen neuen Marketo-Benutzer zu erstellen. Klicken Sie **[!UICONTROL Rollen verwalten]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Markieren Sie **[!UICONTROL Marketo-Synchronisierungsbenutzer]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Wenn Sie die Rolle nicht sehen, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM vorgenommen hat, _nicht_ wieder mit Marketo synchronisiert.

## Marketo-Lösung konfigurieren {#configure-marketo-solution}

Fast fertig! Wir haben nur noch ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Wählen Sie **[!UICONTROL Einstellungen]** aus. Wählen Sie dann **[!UICONTROL Marketo Config]** in der Baumstruktur aus.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht[ veröffentlichen Sie die Marketo-Lösung erneut ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. ![](assets/image2015-4-2-14-3a29-3a1.png) klicken

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Wählen Sie im Popup-Fenster den Synchronisierungsbenutzer aus. Klicken Sie dann auf **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Klicken Sie **[!UICONTROL Speichern]**, um die Änderungen zu speichern.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Klicken Sie auf **[!UICONTROL Alle Anpassungen von Publish]**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, richten [ jetzt einen benutzerdefinierten Synchronisierungsfilter ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Führen Sie den [Microsoft Dynamics-Synchronisierungsprozess ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Es stellt sicher, dass die anfänglichen Setups korrekt ausgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

  Großartig gemacht!

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Microsoft Dynamics mit Marketo verbinden (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
