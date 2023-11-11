---
description: Installieren Sie Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 3 von 3 - Marketo Docs - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 3 von 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 2%

---

# 3. Schritt: Verbinden von Marketo Dynamics (2016 unter Prem/Dynamics 365 On-Premises) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}
>* [Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicks **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Auswählen **[!DNL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicks **[!UICONTROL Bearbeiten]** in **[!UICONTROL Anmeldedaten eingeben]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie die **[!UICONTROL Benutzername]**, **[!UICONTROL Passwort]** Microsoft Dynamics **[!UICONTROL URL]** und ein **Client-ID/Geheimnis**. Klicks **[!UICONTROL Speichern]** wann geschehen.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Wenn Ihre Marketo vor Oktober 2020 bereitgestellt wurde, sind Client-ID und Geheimnis optionale Felder. Andernfalls sind sie obligatorisch. Das Abrufen dieser Informationen hängt von der verwendeten MSD-Version ab.
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer im CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user.
   >* Wenn Sie die URL nicht kennen, [Hier erfahren Sie, wie Sie ihn finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Kennt die URL nicht? Wir zeigen Ihnen, wie Sie Ihre [URL des Dynamics-Organisationsdienstes](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) hier.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicks **[!UICONTROL Bearbeiten]** in **[!UICONTROL Zu synchronisierende Felder auswählen]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit der [Synchronisieren deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, gehen Sie in und wählen Sie die neuen Felder aus, die mit Marketo synchronisiert werden sollen.

1. Navigieren Sie zu Admin und wählen Sie **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicks **[!UICONTROL Bearbeiten]** in den Details zur Feldsynchronisierung.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss &quot;new_synctomkto&quot;lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicks **[!UICONTROL Bearbeiten]** in **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen manuell eingeben.

1. Alles im Popup lesen, Ihre E-Mail eingeben und auf klicken **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-59-51.png)

Exzellente Arbeit!
