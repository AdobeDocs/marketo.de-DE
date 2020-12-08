---
unique-page-id: 3571809
description: Schritt 3 von 3 - Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011) - Marketing Docs - Produktdokumentation
title: Schritt 3 von 3 - Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Gut! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und Dynamics verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren Sie die Marketing Solution (On-Premises 2011)](step-1-of-3-install.md)
>* [Schritt 2 von 3: Einrichten von Marketo Sync User in Dynamics (On-Premises 2011)](step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Dynamics Sync-Benutzerinformationen eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketing an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Klicken Sie auf **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicken Sie in **Schritt 1 auf** Bearbeiten **: Geben Sie Anmeldeinformationen ein.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Vergewissern Sie sich bitte, dass Ihre Anmeldeinformationen korrekt sind, da wir die nachfolgenden Änderungen des Schemas nach der Übermittlung nicht wiederherstellen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketing-Abonnement erhalten.

1. Geben Sie den **Benutzernamen**, das **Kennwort** und die CRM- **URL** ein und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketing muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann &quot; [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) DOMÄNE\Benutzer&quot;lauten.

   >[!TIP]
   >
   >Kennst du die URL nicht? Wir zeigen Ihnen, wie Sie die [Dynamics Organisation Service URL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) finden.

## Zu synchronisierende Felder auswählen {#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, über die wir synchronisieren möchten.

1. Klicken Sie auf **Bearbeiten** in **Schritt 2: Wählen Sie zu synchronisierende Felder aus.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Es gibt vorab ausgewählte Felder, die synchronisiert werden. hinzufügen Sie weitere Informationen und klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## Synchronisieren von Feldern für einen benutzerspezifischen Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerspezifischen Filter erstellt haben, sollten Sie unbedingt einsteigen und die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten** .

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Blättern Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomkto sein, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in **Schritt 3 auf** Bearbeiten **: Aktivieren Sie die Synchronisierung**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch deduplizieren gegen eine Microsoft Dynamics-Synchronisierung, oder wenn Sie manuell eingeben Personen oder Interessenten.

1. Lesen Sie alles im Popup, geben Sie Ihre E-Mail ein und klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisierung kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Exzellente Arbeit!
