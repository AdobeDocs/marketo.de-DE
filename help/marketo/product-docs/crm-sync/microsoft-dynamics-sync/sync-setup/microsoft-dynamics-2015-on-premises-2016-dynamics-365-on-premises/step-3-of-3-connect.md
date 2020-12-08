---
unique-page-id: 7504744
description: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3 - Marketing Docs - Produktdokumentation
title: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 3 von 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}

>[!NOTE]
>
>**Voraussetzungen**
>
>* [Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3](step-1-of-3-install.md)
>* [Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Dynamics Sync-Benutzerinformationen eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketing an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Wählen Sie **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicken Sie in **Schritt 1 auf** Bearbeiten **: Geben Sie Anmeldeinformationen** ein.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Vergewissern Sie sich bitte, dass Ihre Anmeldeinformationen korrekt sind, da wir die nachfolgenden Änderungen des Schemas nach der Übermittlung nicht wiederherstellen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketing-Abonnement erhalten.

1. Geben Sie den **Benutzernamen**, das **Kennwort** eine Microsoft Dynamics- **URL** und eine optionale **Client-ID** ein. Klicken Sie abschließend auf **Speichern** .

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketing muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann &quot; [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1) DOMÄNE\Benutzer&quot;lauten.

   >[!TIP]
   >
   >Kennst du die URL nicht? Wir zeigen Ihnen, wie Sie Ihre [Dynamics Organisation Service URL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) finden.

## Zu synchronisierende Felder auswählen {#select-fields-to-sync}

1. Klicken Sie in **Schritt 2 auf** Bearbeiten **: Wählen Sie zu synchronisierende** Felder aus.

   ![](assets/image2015-3-16-9-51-28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Synchronisieren von Feldern für einen benutzerspezifischen Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerspezifischen Filter erstellt haben, sollten Sie unbedingt einsteigen und die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten** .

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Blättern Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomkto sein, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in **Schritt 3 auf** Bearbeiten **: Aktivieren Sie die Synchronisierung**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch deduplizieren gegen eine Microsoft Dynamics-Synchronisierung, oder wenn Sie manuell eingeben Menschen.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisierung kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-59-51.png)

Exzellente Arbeit!
