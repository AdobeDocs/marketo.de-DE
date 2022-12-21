---
unique-page-id: 3571797
description: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Professional) - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Professional)'
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 10%

---

# Schritt 2 von 3: Salesforce-Benutzer für Marketo (Professional) erstellen {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator ausgeführt werden

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder zu Salesforce (Professional) hinzufügen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

In diesem Artikel passen Sie die Feldberechtigungen mit einem Salesforce-Seitenlayout an und erstellen einen Synchronisierungsbenutzer Marketo-Salesforce .

## Festlegen von Seitenlayouts {#set-page-layouts}

Salesforce Professional legt die Barrierefreiheit auf Feldebene mit Seitenlayouts fest, im Gegensatz zu Salesforce Enterprise/Unlimited-Profilen. Mit diesen Schritten kann der Benutzer für die Marketo-Synchronisierung die benutzerdefinierten Felder aktualisieren.

1. Typ **Seitenlayouts** in der Navigationssuchleiste ohne Drücken der **Eingabe** und klicken Sie auf **Seitenlayout** under **Leads**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicken **Bearbeiten** neben Lead-Layout.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicken und ziehen Sie eine neue **Abschnitt** in das Seitenlayout ein.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Geben Sie &quot;Marketo&quot;ein für **Bereichsname** und klicken Sie auf **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicken und ziehen Sie das Feld **Akquisedatum** in **Marketo** Abschnitt.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Wiederholen Sie den obigen Schritt für die folgenden Felder:

   * Akquirierungsprogramm
   * Akquisitionsprogramm-ID
   * E-Mail-Abmeldung
   * Abgeleiteter Ort
   * Abgeleitetes Unternehmen
   * Abgeleitetes Land
   * Abgeleiteter Stadtbereich
   * Abgeleitete Vorwahl
   * Abgeleitete Postleitzahl
   * Abgeleitetes Bundesland/abgeleitete Region
   * Lead-Bewertung
   * Ursprünglicher Verweis
   * Ursprüngliche Such-Engine
   * Ursprünglicher Suchausdruck
   * Ursprüngliche Quelleninfo
   * Ursprünglicher Quellentyp

   >[!NOTE]
   >
   >Diese Felder müssen im Seitenlayout vorhanden sein, damit Marketo sie lesen/schreiben kann.

   >[!TIP]
   >
   >Erstellen Sie zwei Spalten für die Felder, indem Sie sie nach rechts auf der Seite ziehen. Sie können Felder von einer Seite zur anderen verschieben, um die Spaltenlängen auszugleichen.

1. Klicken **Speichern** wenn das Hinzufügen von Feldern abgeschlossen ist.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Wiederholen Sie alle oben genannten Schritte für Salesforce **Kontaktseitenlayout**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Denken Sie daran, auf **Speichern** wenn Sie mit dem **Kontaktseitenlayout**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die Variable **Ganztägige Veranstaltung** wurde dem **Layout der Ereignisseite**.

## Synchronisierungsbenutzer erstellen {#create-sync-user}

Marketo benötigt Anmeldeinformationen für den Zugriff auf Salesforce. Dies sollte am besten mit einem dedizierten Benutzer durchgeführt werden, der mit den folgenden Schritten erstellt wurde.

>[!NOTE]
>
>Wenn Ihre Organisation über keine zusätzlichen Salesforce-Lizenzen verfügt, können Sie eine vorhandene **Marketing-Benutzer** mit dem **Systemadministrator** Profil.

1. Geben Sie &quot;Benutzer&quot;in die Navigationssuchleiste ein und klicken Sie auf **Benutzer** under **Benutzer verwalten**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicken **Neuer Benutzer**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Füllen Sie die erforderlichen Felder aus und wählen Sie die **Anwenderlizenz: Salesforce**, legen Sie die **Profil: Systemadministrator**, check **Marketing-Benutzer** und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Vergewissern Sie sich, dass die von Ihnen eingegebene E-Mail-Adresse gültig ist. Sie müssen sich als Synchronisierungsbenutzer anmelden, um das Kennwort zurückzusetzen.

Ausgezeichnet! Jetzt haben Sie ein Konto, mit dem Marketo eine Verbindung zu Salesforce herstellen kann. Machen wir es!

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Verbinden von Marketo und Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
