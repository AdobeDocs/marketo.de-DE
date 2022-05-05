---
description: 'Schritt 3 von 3: Verbinden von Marketo Engage- und VEC-CRM - Marketo-Dokumente - Produktdokumentation'
title: 3. Schritt - Marketo Engage- und Veeva-CRM verbinden
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Schritt 3 von 3: Marketo Engage- und Veeva-CRM verbinden {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

In diesem Artikel konfigurieren Sie Marketo Engage so, dass es mit Ihrer konfigurierten VEE CRM-Instanz synchronisiert wird. **Salesforce wird in einigen Popups angezeigt** da Veeva CRM auf der Salesforce-Plattform basiert.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu VEC](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}
>* [Schritt 2 von 3: Erstellen eines VEC-Benutzers für Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target=&quot;_blank&quot;}


>[!IMPORTANT]
>
>Es kann jeweils nur eine Marketo-Instanz mit einer Veeva CRM-Instanz verbunden werden.

## Verbindung mit VEeva CRM über OAuth herstellen {#connect-to-veeva-crm-using-oauth}

1. Klicken Sie in Marketo auf **Admin**. Auswählen **CRM** und klicken Sie auf **Mit Veeva synchronisieren**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass [Alle nicht benötigten Felder ausblenden](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target=&quot;_blank&quot;} in Marketo vom Synchronisierungsbenutzer aus, bevor auf &quot;Synchronisierungsfelder&quot;geklickt wird. Wenn Sie auf Felder synchronisieren klicken, werden alle Felder, die dem Benutzer angezeigt werden, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Klicken **Bei Veeva anmelden**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Aktivieren Sie Sandbox , wenn Sie eine Marketo-Sandbox mit einer VEA CRM-Sandbox synchronisieren.

1. Klicken **Anmeldeinformationen bestätigen**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Ein Popup mit der Salesforce-Anmeldeseite wird angezeigt. Geben Sie Ihre Anmeldedaten für &quot;Marketo Sync User&quot;ein und klicken Sie auf **Anmelden**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Geben Sie den Verifikationscode ein, den Sie per E-Mail erhalten haben (von Salesforce gesendet), und klicken Sie auf **Überprüfen**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Nach erfolgreicher Überprüfung wird auf der Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicken **Zulassen**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. In einigen Minuten wird ein Popup in Marketo Enge angezeigt. Klicken **Anmeldeinformationen bestätigen**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Starten der VEC-Synchronisierung {#start-veeva-sync}

1. Klicken **Starten der VEC-Synchronisierung** um die permanente Marketo-Veeva CRM-Synchronisation zu starten.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert das Duplizieren nicht automatisch für eine VEE CRM-Synchronisation oder wenn Sie Leads manuell eingeben.

1. Klicken **Synchronisierung starten**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Die Dauer der Erstsynchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die VEA CRM-Synchronisation im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **Admin**, dann **Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Der Synchronisierungsstatus wird oben rechts angezeigt. Es wird eine von drei Nachrichten angezeigt: Letzte Synchronisierung, Synchronisierung läuft oder Fehlgeschlagen.

>[!MORELIKETHIS]
>
>[Benutzerdefinierte Objekte konfigurieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}
