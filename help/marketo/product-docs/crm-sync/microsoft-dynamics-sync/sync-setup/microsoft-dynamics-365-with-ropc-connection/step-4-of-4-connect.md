---
description: 'Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortkontrollverbindung für Ressourcenbesitzer - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers'
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 3%

---

# Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers {#step-4-of-4-connect-the-marketo-solution-ropc}

Dies ist der letzte Schritt der Synchronisierung. Sie haben es fast geschafft!

>[!PREREQUISITES]
>
>* [Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Schritt 2 von 4: Richten Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung für Ressourcenbesitzer ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Schritt 3 von 4: Einrichten der Client-App auf MS [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Wenn Sie ein Upgrade von der einfachen Authentifizierung auf [!DNL OAuth] durchführen, können Sie [diesen Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) verwenden, um Ihre Authentifizierung neu zu konfigurieren.

## Benutzerinformationen für [!DNL Dynamics] eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 1: Anmeldeinformationen eingeben]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Organisations-URL korrekt ist, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn eine falsche Org-URL verwendet wird, müssen Sie ein neues Marketo-Abonnement erwerben. Wenn Sie die URL nicht kennen, ([&#x200B; Sie hier, wie Sie sie finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!NOTE]
   >
   >Bevor Sie neue Anmeldeinformationen eingeben, können [&#x200B; sie hier &#x200B;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

1. Geben Sie **[!UICONTROL Benutzername]**, **[!UICONTROL Kennwort]**, [!DNL Microsoft Dynamics] **[!UICONTROL URL]**, **[!UICONTROL Client-ID]** und **[!UICONTROL Client-Geheimnis]** ein. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user lauten.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 2: Auswahl der zu synchronisierenden Felder]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die mit Marketo synchronisiert werden sollen, sodass sie vorausgewählt sind. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in [!DNL Dynamics] löschen, wird empfohlen, dies mit [Synchronisierung deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Option [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md) bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, müssen Sie die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Wechseln Sie zu [!UICONTROL Admin] und wählen Sie **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** auf [!UICONTROL Details zur Feldsynchronisierung].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomito lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 3: Synchronisierung aktivieren]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine [!UICONTROL Microsoft Dynamics]-Synchronisierung dedupliziert oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail-Adresse ein und klicken Sie auf **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Je nach Anzahl der Datensätze kann die erste Synchronisierung einige Stunden bis zu einige Tage dauern. Nach Abschluss erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[Authentifizierungsmethode  [!DNL Dynamics] Neu konfigurieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
