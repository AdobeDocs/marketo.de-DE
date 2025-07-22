---
description: Schritt 3 von 3 - Marketo Engage und  [!DNL Veeva] -CRM verbinden - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 3 von 3: Marketo Engage und  [!DNL Veeva]  verbinden'
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Schritt 3 von 3: Marketo Engage und [!DNL Veeva] CRM verbinden {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

In diesem Artikel konfigurieren Sie Marketo Engage für die Synchronisierung mit Ihrer konfigurierten [!DNL Veeva] CRM-Instanz. **Sie werden [!DNL Salesforce] in einigen der Pop-ups sehen** da [!DNL Veeva] CRM auf der [!DNL Salesforce] Plattform erstellt wird.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Marketo-Felder hinzufügen zu [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Schritt 2 von 3: Erstellen eines  [!DNL Veeva]  für Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Es kann jeweils nur eine Marketo-Instanz mit einer [!DNL Veeva] CRM-Instanz verbunden werden.

## Verbindung mit [!DNL Veeva] CRM über OAuth herstellen {#connect-to-veeva-crm-using-oauth}

1. Klicken Sie in Marketo auf **[!UICONTROL admin]**. Wählen Sie **[!UICONTROL CRM]** und klicken Sie auf **[!UICONTROL Mit Veeva synchronisieren]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Stellen Sie sicher[ dass Sie in Marketo alle nicht benötigten Felder ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} Synchronisierungsbenutzer ausblenden, bevor Sie auf „Felder synchronisieren“ klicken. Nachdem Sie auf Felder synchronisieren geklickt haben, werden alle Felder, die der Benutzer sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Klicken Sie **[!UICONTROL Mit Veeva anmelden]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Aktivieren Sie [!UICONTROL Sandbox], wenn Sie eine Marketo-Sandbox mit einer [!DNL Veeva] CRM-Sandbox synchronisieren.

1. Klicken Sie **[!UICONTROL Anmeldedaten bestätigen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Es wird ein Popup mit der Anmeldeseite von [!DNL Salesforce] angezeigt. Geben Sie Ihre &quot;Marketo Sync User“-Anmeldedaten ein und klicken Sie **[!UICONTROL Anmelden]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Geben Sie den Bestätigungscode ein, den Sie per E-Mail erhalten haben (gesendet von [!DNL Salesforce]), und klicken Sie auf **[!UICONTROL Überprüfen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Nach erfolgreicher Überprüfung wird die Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicken Sie **[!UICONTROL Zulassen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. In einigen Minuten wird ein Popup in Marketo Engage angezeigt. Klicken Sie **[!UICONTROL Anmeldedaten bestätigen]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Starten [!DNL Veeva] Synchronisierung {#start-veeva-sync}

1. Klicken Sie **[!UICONTROL Veeva Sync starten]**, um die persistente [!DNL Marketo-Veeva] CRM-Synchronisierung zu starten.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine [!DNL Veeva] CRM-Synchronisation dedupliziert oder wenn Sie Leads manuell eingeben.

1. Klicken Sie **[!UICONTROL Synchronisierung starten]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Die Zeit bis zum Abschluss der ersten Synchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die [!DNL Veeva] CRM-Synchronisation im Admin-Bereich bereit. Gehen Sie wie folgt vor, um zu überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert.

1. Klicken Sie in Marketo **[!UICONTROL Admin]** gefolgt von **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Der Synchronisierungsstatus wird in der oberen rechten Ecke angezeigt. Daraufhin wird eine der drei Meldungen angezeigt: Zuletzt synchronisiert, Synchronisierung läuft oder Fehlgeschlagen.

>[!MORELIKETHIS]
>
>[Benutzerdefinierte Objekte konfigurieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
