---
unique-page-id: 3571816
description: 'Schritt 2 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013) - Marketo Docs - Produktdokumentation'
title: Schritt 2 von 3 - Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Schritt 2 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Gute Arbeit, die vorherigen Schritte abzuschließen, lassen Sie uns weiter durchgehen.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"}

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für das Marketo-Plug-in Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch eingestellt sein](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. under **Einstellungen** klicken **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Auswählen **Benutzer**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Hier sehen Sie eine Liste der Benutzer. Wählen Sie den dedizierten Marketo Sync-Benutzer aus oder kontaktieren Sie Ihren [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} administrator to create a new user that's [dedicated to Marketo](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx){target="_blank"}.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicks ![](assets/image2015-3-26-11-3a16-3a22.png) und wählen **[!UICONTROL Rollen verwalten]**.

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Überprüfen **[!UICONTROL Marketo Sync User]** und klicken **[!UICONTROL OK]**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"} und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden _not_ wieder mit Marketo synchronisiert werden.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast fertig! Wir haben nur einige letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. under **[!UICONTROL Einstellungen]** klicken **[!UICONTROL Marketo-Konfiguration]**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Wenn &quot;Marketo-Konfiguration&quot;fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, [Marketo-Lösung veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) erneut oder versuchen Sie, sich ab- und wieder anzumelden.

1. Klicks **[!UICONTROL Standard]**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicken Sie auf **[!UICONTROL Marketo-Benutzer]** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicks ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicks **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, [Einrichten eines benutzerdefinierten Synchronisierungsfilters](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} jetzt.
* Führen Sie die [Überprüfen der Synchronisierung mit Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -Prozess. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

Gut gemacht!

>[!MORELIKETHIS]
>
>[3. Schritt: Marketo und Dynamics verbinden (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md){target="_blank"}
