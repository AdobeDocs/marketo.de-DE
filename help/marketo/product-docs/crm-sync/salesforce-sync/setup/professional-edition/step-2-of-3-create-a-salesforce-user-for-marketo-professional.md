---
unique-page-id: 3571797
description: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketo (Professional) - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Professional)'
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Schritt 2 von 3: Erstellen eines [!DNL Salesforce] für Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator durchgeführt werden.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder zu Salesforce (Professional) hinzufügen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

In diesem Artikel passen Sie Feldberechtigungen mit einem [!DNL Salesforce] Seitenlayout an und erstellen einen Marketo-[!DNL Salesforce] Synchronisierungsbenutzer.

## Festlegen von Seiten-Layouts {#set-page-layouts}

[!DNL Salesforce] Professional legt die Barrierefreiheit auf Feldebene mit Seiten-Layouts im Gegensatz zu den Profilen von [!DNL Salesforce] Enterprise/Unlimited fest. Mit diesen Schritten kann der Marketo-Synchronisierungsbenutzer die benutzerdefinierten Felder aktualisieren.

1. Geben Sie &quot;[!UICONTROL Seitenlayouts]&quot; in die Navigationssuchleiste ein, ohne die **[!UICONTROL Eingabetaste]** zu drücken, und klicken Sie auf **[!UICONTROL Seitenlayout]** unter **[!UICONTROL Leads]**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** neben Lead-Layout.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicken Sie auf und ziehen Sie einen neuen **[!UICONTROL Abschnitt]** in das Seitenlayout.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Geben Sie &quot;Marketo&quot; für **[!UICONTROL Abschnittsname]** ein und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicken Sie auf und ziehen Sie das Feld **[!UICONTROL Akquisitionsdatum]** in den Abschnitt **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Wiederholen Sie den obigen Schritt für die folgenden Felder:

   * [!UICONTROL Akquise-Programm]
   * [!UICONTROL Akquise-Programm-ID]
   * [!UICONTROL E-Mail-Opt-out]
   * [!UICONTROL Abgeleitete Stadt]
   * [!UICONTROL Abgeleitetes Unternehmen]
   * [!UICONTROL Abgeleitetes Land]
   * [!UICONTROL Geschätzte Metropolregion]
   * [!UICONTROL Abgeleitete Telefonvorwahl]
   * [!UICONTROL Abgeleitete Postleitzahl]
   * [!UICONTROL Abgeleitete Statusregion]
   * [!UICONTROL Lead-Bewertung]
   * [!UICONTROL Ursprünglicher Referrer]
   * [!UICONTROL Original-Suchmaschine]
   * [!UICONTROL Ursprüngliche Suchphrase]
   * [!UICONTROL Original Source Info]
   * [!UICONTROL Original-Source-Typ]

   >[!NOTE]
   >
   >Diese Felder müssen sich im Seiten-Layout befinden, damit Marketo sie lesen/schreiben kann.

   >[!TIP]
   >
   >Erstellen Sie zwei Spalten für die Felder, indem Sie sie nach unten auf die rechte Seite ziehen. Sie können Felder von einer Seite auf die andere verschieben, um die Spaltenlängen auszugleichen.

1. Klicken Sie auf **[!UICONTROL Speichern]** wenn Sie das Hinzufügen von Feldern abgeschlossen haben.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Wiederholen Sie alle oben genannten Schritte für das Salesforce **[!UICONTROL Kontaktseiten-Layout]**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Denken Sie daran **[!UICONTROL auf &quot;]**&quot; zu klicken, wenn Sie mit dem **[!UICONTROL Kontaktseiten-Layout]** fertig sind.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Stellen Sie sicher **[!UICONTROL dass das Feld]** Ganztägiges Ereignis“ zum **[!UICONTROL Ereignisseiten-Layout“ hinzugefügt]**.

## Synchronisierungsbenutzer erstellen {#create-sync-user}

Marketo benötigt Anmeldeinformationen, um auf [!DNL Salesforce] zuzugreifen. Dies geschieht am besten mit einem dedizierten Benutzer, der mit den folgenden Schritten erstellt wurde.

>[!NOTE]
>
>Wenn Ihr Unternehmen über keine zusätzlichen Salesforce-Lizenzen verfügt, können Sie einen bestehenden Marketing-Benutzer mit dem Systemadministratorprofil verwenden.

1. Geben Sie in der Navigationssuchleiste „Benutzer“ ein und klicken Sie unter **[!UICONTROL Benutzer verwalten]** auf **[!UICONTROL Benutzer]**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicken Sie auf **[!UICONTROL Neuer Benutzer]**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Füllen Sie die erforderlichen Felder aus, wählen Sie **[!UICONTROL Benutzerlizenz: Salesforce]**, legen Sie **[!UICONTROL Profil:]** fest, aktivieren Sie **[!UICONTROL Marketing-Benutzer]** und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass die eingegebene E-Mail-Adresse gültig ist. Sie müssen sich als Synchronisierungsbenutzer anmelden, um das Kennwort zurückzusetzen.

Ausgezeichnet! Jetzt verfügen Sie über ein Konto, mit dem Marketo eine Verbindung zu [!DNL Salesforce] herstellen kann. Lass es uns machen.

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Marketo und Salesforce verbinden (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
