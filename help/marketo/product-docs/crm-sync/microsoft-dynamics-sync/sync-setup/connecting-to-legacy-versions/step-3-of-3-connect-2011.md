---
unique-page-id: 3571809
description: Schritt 3 von 3 -  [!DNL Microsoft Dynamics]  mit Marketo (2011 On-Premise) - Marketo-Dokumente - Produktdokumentation
title: Schritt 3 von 3 - Verbinden  [!DNL Microsoft Dynamics]  Marketo (2011 On-Premise)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 2%

---

# Schritt 3 von 3: Verbinden von [!DNL Microsoft Dynamics] mit Marketo (2011 On-Premise) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

In Ordnung! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und [!DNL Dynamics] verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketo-Lösung (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [Schritt 2 von 3: Einrichten von Marketo Sync User in [!DNL Dynamics] (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Benutzerinformationen für [!DNL Dynamics] eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Auf **[!UICONTROL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 1: Anmeldeinformationen eingeben]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie **[!UICONTROL Benutzername]**, **[!UICONTROL Kennwort]** und CRM-**[!UICONTROL URL ein]** klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Der [!UICONTROL Benutzername] in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user lauten.
   >* Wenn Sie die URL nicht kennen, ([ Sie hier, wie Sie sie finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, die wir synchronisieren möchten.

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 2: Auswahl der zu synchronisierenden Felder]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Es gibt vorab ausgewählte Felder, die synchronisiert werden. Fügen Sie bei Bedarf weitere hinzu und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in [!DNL Dynamics] löschen, wird empfohlen, dies mit [Synchronisierung deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Option [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md) bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, müssen Sie die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Wechseln Sie zu Admin und wählen Sie **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** auf [!UICONTROL Details zur Feldsynchronisierung].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomito lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 3: Synchronisierung aktivieren]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine [!DNL Microsoft Dynamics]-Synchronisierung dedupliziert oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Je nach Anzahl der Datensätze kann die erste Synchronisierung einige Stunden bis zu einige Tage dauern. Nach Abschluss erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)
