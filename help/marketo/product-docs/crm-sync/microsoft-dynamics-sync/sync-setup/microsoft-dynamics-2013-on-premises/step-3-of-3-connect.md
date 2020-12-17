---
unique-page-id: 3571819
description: Schritt 3 von 3 - Connect Marketing and Dynamics (On-Premises 2013) - Marketing Docs - Produktdokumentation
title: Schritt 3 von 3 - Connect Marketing and Dynamics (On-Premises 2013)
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# Schritt 3 von 3: Connect Marketing and Dynamics (On-Premises 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Gut! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und Dynamics verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren Sie die Marketing Solution in Dynamics (On-Premises 2013)](step-1-of-3-install.md)
>* [Schritt 2 von 3: Konfigurieren des Synchronisierungsbenutzers für Marketo (On-Premises 2013)](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Dynamics Sync-Benutzerinformationen eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketing an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Wählen Sie **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicken Sie in **Schritt 1 auf** BEARBEITEN **: Geben Sie Anmeldeinformationen** ein.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Vergewissern Sie sich bitte, dass Ihre Anmeldeinformationen korrekt sind, da wir die nachfolgenden Änderungen des Schemas nach der Übermittlung nicht wiederherstellen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketing-Abonnement erhalten.

1. Geben Sie **Benutzername**, **Kennwort** und Microsoft Dynamics **URL** ein und klicken Sie dann auf **Speichern**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketing muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann &quot;[`[email protected]`&quot;oder &quot;](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e)&quot;oder &quot;DOMAIN\user&quot;lauten.

   >[!TIP]
   >
   >Kennst du die URL nicht? Wir zeigen Ihnen, wie Sie die [Dynamics Organisationsdienst-URL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) hier finden.

## Zu synchronisierende Felder auswählen{#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, über die wir synchronisieren möchten.

1. Klicken Sie auf **BEARBEITEN **in **Schritt 2: Wählen Sie die zu synchronisierenden Felder aus.**

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Synchronisieren von Feldern für einen benutzerspezifischen Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerspezifischen Filter erstellt haben, sollten Sie unbedingt einsteigen und die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten**.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Blättern Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomkto sein, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie auf **BEARBEITEN **in **Schritt 3: Aktivieren Sie die Synchronisierung**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch deduplizieren gegen eine Microsoft Dynamics-Synchronisierung, oder wenn Sie manuell eingeben Personen oder Interessenten.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **BEGINN SYNC**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisierung kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Exzellente Arbeit! Sie haben soeben die Kraft der bidirektionalen Synchronisierung zwischen Marketo und Microsoft Dynamics freigesetzt. Wenn Sie Marketo Sales Insight gekauft haben, haben Sie mehr Spaß:

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



