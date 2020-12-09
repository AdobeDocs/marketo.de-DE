---
unique-page-id: 3571800
description: Schritt 3 von 3 - Connect Marketing and Salesforce (Professional) - Marketing Docs - Produktdokumentation
title: Schritt 3 von 3 - Connect Marketing and Salesforce (Professional)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# Schritt 3 von 3: Connect Marketing und Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In diesem Artikel konfigurieren Sie Marketo für die Synchronisierung mit Ihrer konfigurierten Salesforce-Instanz.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: hinzufügen Marketo Fields to Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketing (Professional)](step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

>



## Synchronisierungs-Sicherheits-Token abrufen {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie direkt mit &quot;Synchronisieren Sie Benutzeranmeldeinformationen und -kudos für die Vorbereitung!&quot;fort.

1. Melden Sie sich bei Salesforce mit dem Marketo Sync User an, klicken Sie auf den Namen des Synchronisierungsbenutzers und dann auf **Meine Einstellungen**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Geben Sie in der Navigationsleiste &quot;reset&quot;ein und klicken Sie auf &quot; **Reset My Security Token&quot;**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Klicken Sie auf Sicherheitstoken **zurücksetzen**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Das Sicherheitstoken wird Ihnen per E-Mail zugesendet.

## Benutzeranmeldeinformationen synchronisieren {#set-sync-user-credentials}

1. Gehen Sie in Marketo zu **Admin**, wählen Sie **CRM** und klicken Sie auf **Synchronisieren mit [Salesforce.com](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Vergewissern Sie sich, dass Sie alle Felder, die Sie in Marketing nicht benötigen [, vor dem Synchronisierungsbenutzer](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) ausblenden, bevor Sie auf &quot;Felder **synchronisieren&quot;klicken**. Nachdem Sie auf &quot;Felder synchronisieren&quot;geklickt haben, werden alle Felder, die der Benutzer sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die in Teil 2 der Salesforce-Konfiguration ([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW), [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW)) erstellten Salesforce Sync User-Anmeldedaten ein und klicken Sie auf **Synchronisierungsfelder**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Markieren Sie **Sandbox** , wenn Sie eine Marketo Sandbox mit einer Salesforce Sandbox synchronisieren.

1. Lesen Sie die Warnung und klicken Sie dann auf Anmeldeinformationen **bestätigen**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie über die [Zuordnungen schauen und sie](../../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)anpassen möchten, ist dies Ihre einzige Chance! Nachdem Sie auf Beginn Salesforce Sync geklickt haben, ist es fertig.

## Beginn Salesforce Sync {#start-salesforce-sync}

1. Klicken Sie auf **Beginn Salesforce Sync** , um die permanente Synchronisierung von Marketing-Salesforce zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo wird die Duplizierung nicht automatisch bei einer Salesforce-Synchronisierung oder bei manueller Eingabe von Leads aufheben.

1. Klicken Sie auf **BEGINN SYNC**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Die Dauer zum Abschluss der ersten Synchronisierung hängt von der Größe und Komplexität der Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die Salesforce-Synchronisierung im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **Admin** und dann auf **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Der Synchronisierungsstatus ist in der oberen rechten Ecke sichtbar. Es wird eine von drei Nachrichten angezeigt: **Letzte Synchronisierung**, **Synchronisierung läuft** oder **Fehlgeschlagen**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, du hast gerade eine der mächtigsten Funktionen von Marketo konfiguriert, los!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>* [Optionale Schritte](http://docs.marketo.com/display/docs/optional+steps)

>



