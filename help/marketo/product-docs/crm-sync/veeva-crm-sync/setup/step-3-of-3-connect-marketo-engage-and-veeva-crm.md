---
description: 'Schritt 3 von 3: Verbinden von Marketo Engage- und Veeva CRM - Marketo Docs - Produktdokumentation'
title: 3. Schritt - Marketo Engage- und Veeva-CRM verbinden
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 3. Schritt: Marketo Engage und Veeva CRM verbinden {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

In diesem Artikel konfigurieren Sie Marketo Engage zur Synchronisierung mit Ihrer konfigurierten VEE CRM-Instanz. **Salesforce wird in einigen Popups angezeigt** da Veeva CRM auf der Salesforce-Plattform basiert.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Marketo-Felder zu Veeva hinzufügen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Schritt 2 von 3: Erstellen eines VEC-Benutzers für Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Es kann jeweils nur eine Marketo-Instanz mit einer Veeva CRM-Instanz verbunden werden.

## Verbindung mit VEeva CRM über OAuth herstellen {#connect-to-veeva-crm-using-oauth}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**. Auswählen **[!UICONTROL CRM]** und klicken **[!UICONTROL Mit Veeva synchronisieren]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, [Alle nicht benötigten Felder ausblenden](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo vom Synchronisierungsbenutzer aus, bevor Sie auf &quot;Synchronisierungsfelder&quot;klicken. Wenn Sie auf Felder synchronisieren klicken, werden alle Felder, die dem Benutzer angezeigt werden, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Klicks **[!UICONTROL Bei Veeva anmelden]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Aktivieren Sie Sandbox , wenn Sie eine Marketo-Sandbox mit einer VEA CRM-Sandbox synchronisieren.

1. Klicks **[!UICONTROL Anmeldeinformationen bestätigen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Ein Popup mit der Salesforce-Anmeldeseite wird angezeigt. Geben Sie Ihre Anmeldedaten für Marketo Sync User ein und klicken Sie auf **[!UICONTROL Anmelden]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Geben Sie den Verifikationscode ein, den Sie per E-Mail erhalten haben (von Salesforce gesendet), und klicken Sie auf **[!UICONTROL Überprüfen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Nach erfolgreicher Überprüfung wird auf der Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicks **[!UICONTROL Zulassen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. In einigen Minuten wird ein Popup in Marketo Enge angezeigt. Klicks **[!UICONTROL Anmeldeinformationen bestätigen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Starten der VEC-Synchronisierung {#start-veeva-sync}

1. Klicks **[!UICONTROL Starten der VEC-Synchronisierung]** um die permanente Marketo-Veeva CRM-Synchronisation zu starten.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert das Duplizieren nicht automatisch für eine VEE CRM-Synchronisation oder wenn Sie Leads manuell eingeben.

1. Klicks **[!UICONTROL Synchronisierung starten]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Die Dauer der Erstsynchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die VEA CRM-Synchronisation im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**, dann **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Der Synchronisierungsstatus wird oben rechts angezeigt. Es wird eine von drei Meldungen angezeigt: &quot;Zuletzt synchronisiert&quot;, &quot;Synchronisierung läuft&quot;oder &quot;Fehlgeschlagen&quot;.

>[!MORELIKETHIS]
>
>[Benutzerdefinierte Objekte konfigurieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
