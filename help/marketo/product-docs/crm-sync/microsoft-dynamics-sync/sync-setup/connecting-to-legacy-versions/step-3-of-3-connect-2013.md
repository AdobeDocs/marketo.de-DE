---
unique-page-id: 3571819
description: Schritt 3 von 3 - Marketo und Dynamics verbinden (2013 On-Premise) - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 3 von 3: Verbinden von Marketo und Dynamics (2013 On-Premise)'
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 2%

---

# Schritt 3 von 3: Marketo und [!DNL Dynamics] verbinden (2013 On-Premise) {#step-of-connect-marketo-and-dynamics-on-premises}

In Ordnung! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und [!DNL Dynamics] verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketo-Lösung in  [!DNL Dynamics] (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [Schritt 2 von 3: Konfigurieren von Synchronisierungsbenutzenden für Marketo (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Benutzerinformationen für [!DNL Dynamics] eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Wählen Sie **[!DNL Microsoft]** aus.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 1: Anmeldeinformationen eingeben]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie **[!UICONTROL Benutzername]**, **[!UICONTROL Kennwort]** und [!DNL Microsoft Dynamics] **URL ein** klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user lauten.
   >* Wenn Sie die URL nicht kennen, ([ Sie hier, wie Sie sie finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, die wir synchronisieren möchten.

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 2: Auswahl der zu synchronisierenden Felder]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die mit Marketo synchronisiert werden sollen, sodass sie vorausgewählt sind. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in [!DNL Dynamics] löschen, wird empfohlen, dies mit [Synchronisierung deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Option [[!UICONTROL Zu synchronisierende Felder auswählen]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md) bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, müssen Sie die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Wechseln Sie zu [!UICONTROL Admin] und wählen Sie **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** auf [!UICONTROL Details zur Feldsynchronisierung].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomito lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie **[!UICONTROL Bearbeiten]** in **[!UICONTROL Schritt 3: Synchronisierung aktivieren]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine [!DNL Microsoft Dynamics]-Synchronisierung dedupliziert oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Je nach Anzahl der Datensätze kann die erste Synchronisierung einige Stunden bis zu einige Tage dauern. Nach Abschluss erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Hervorragende Arbeit! Sie haben soeben die Leistungsfähigkeit der bidirektionalen Synchronisation zwischen Marketo und [!DNL Microsoft Dynamics] entfesselt. Wenn Sie [!DNL Marketo Sales Insight] gekauft haben, gibt es mehr Spaß zu haben:

>[!MORELIKETHIS]
>
>[Installieren und Konfigurieren [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics] 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
