---
description: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premise - Schritt 3 von 3 - Dokumente zu Marketo - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premise, Schritt 3 von 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 3%

---

# Schritt 3 von 3: Marketo Dynamics verbinden (2016 On-Premise/Dynamics 365 On-Premise) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premise, Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}
>* [Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premise - Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Dynamics-Sync-Benutzerinformationen eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Wählen Sie **[!DNL Microsoft]** aus.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Anmeldedaten eingeben]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie **[!UICONTROL Benutzername]**, **[!UICONTROL Kennwort]** eine Microsoft Dynamics **[!UICONTROL URL]** und eine **Client-ID/-** ein. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Wenn Ihre Marketo vor Oktober 2020 bereitgestellt wurde, sind Client-ID und Geheimnis optionale Felder. Andernfalls sind sie obligatorisch. Der Erhalt dieser Informationen hängt davon ab, welche Version von MSD Sie verwenden.
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user lauten.
   >* Wenn Sie die URL nicht kennen, ([ Sie hier, wie Sie sie finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Kennst du die URL nicht? Wir zeigen Ihnen hier, wie Sie Ihre [Dynamics-Organisationsdienst-URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) finden.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Felder zum Synchronisieren auswählen]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Wählen Sie die Felder aus, die mit Marketo synchronisiert werden sollen, sodass sie vorausgewählt sind. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit deaktivierter [Synchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"} durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Option [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"} bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, müssen Sie die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **[!DNL Microsoft Dynamics]** aus.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** auf Details zur Feldsynchronisierung.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomito lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine Microsoft Dynamics-Synchronisierung dedupliziert oder wenn Sie Personen manuell eingeben.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Je nach Anzahl der Datensätze kann die erste Synchronisierung einige Stunden bis zu einige Tage dauern. Nach Abschluss erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-59-51.png)
