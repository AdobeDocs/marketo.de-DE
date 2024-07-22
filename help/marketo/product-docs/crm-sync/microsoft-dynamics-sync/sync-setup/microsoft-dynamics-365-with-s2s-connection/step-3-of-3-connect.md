---
unique-page-id: 3571830
description: 'Schritt 3: Verbinden der Marketo-Lösung mit der Server-Verbindung - Marketo Docs - Produktdokumentation'
title: 'Schritt 3: Verbinden der Marketo-Lösung mit der Server-zu-Server-Verbindung'
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 2%

---

# Schritt 3: Verbinden der Marketo-Lösung mit der Server-zu-Server-Verbindung {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Dies ist der letzte Schritt der Synchronisierung. Wir sind fast da!

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketo-Lösung mit Server-zu-Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}
>* [Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!IMPORTANT]
>
>Wenn Sie von der einfachen Authentifizierung auf OAuth aktualisieren, müssen Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} wenden, um Hilfe beim Aktualisieren der zusätzlichen Parameter zu erhalten. Durch Aktivierung dieser Funktion wird die Synchronisierung vorübergehend angehalten, bis neue Anmeldeinformationen eingegeben und die Synchronisierung wieder aktiviert wird. Die Funktion kann (bis April 2022) deaktiviert werden, wenn Sie zum alten Authentifizierungsmodus zurückkehren möchten.

>[!NOTE]
>
>Bevor Sie neue Anmeldedaten eingeben, können Sie diese hier [validieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Wählen Sie **[!DNL Microsoft]** aus.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]** in **[!UICONTROL Anmeldedaten eingeben]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Organisations-URL korrekt ist, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn eine falsche Organisations-URL verwendet wird, müssen Sie ein neues Marketo-Abonnement erhalten. Wenn Sie die URL nicht kennen, erfahren Sie [, wie Sie sie hier finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

1. Geben Sie die Benutzerinformationen für die Dynamics Sync ein und klicken Sie danach auf **[!UICONTROL Speichern]** .

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketo muss mit der [E-Mail-Adresse](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} des Anwendungsbenutzers im CRM-System übereinstimmen. Das Format kann &quot;`user@domain.com`&quot; oder &quot;DOMAIN\user&quot; lauten.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicken Sie auf **[!UICONTROL Bearbeiten]** in **[!UICONTROL Zu synchronisierende Felder auswählen]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit der deaktivierten [Synchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"} durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die [Zu synchronisierenden Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"} bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, gehen Sie in und wählen Sie die neuen Felder aus, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **[!DNL Microsoft Dynamics]** aus.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie in den Details zur Feldsynchronisierung auf **[!UICONTROL Bearbeiten]** .

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss &quot;new_synctomkto&quot;lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in **[!UICONTROL Synchronisation aktivieren]** auf **[!UICONTROL Bearbeiten]** .

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup-Fenster, geben Sie Ihre E-Mail-Adresse ein und klicken Sie auf **[!UICONTROL Synchronisation starten]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Exzellente Arbeit!
