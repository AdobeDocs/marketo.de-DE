---
unique-page-id: 3571797
description: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketing (Professional) - Marketing Docs - Produktdokumentation
title: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketing (Professional)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketing (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator ausgeführt werden

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: hinzufügen Marketo Fields to Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



In diesem Artikel passen Sie die Feldberechtigungen mit einem Salesforce-Seitenlayout an und erstellen einen Synchronisierungsbenutzer von &quot;Marketing-Salesforce&quot;.

## Seitenlayouts festlegen {#set-page-layouts}

Salesforce Professional stellt die Barrierefreiheit auf Feldebene mit Seitenlayouts ein, im Gegensatz zu Salesforce Enterprise/Unlimited Profilen. Wenn Sie diese Schritte ausführen, kann der Benutzer mit der Synchronisierung die benutzerdefinierten Felder aktualisieren.

1. Geben Sie **Seitenlayouts** in der Navigationsleiste ein, ohne die **Eingabetaste** zu drücken, und klicken Sie unter &quot; **Interessenten** &quot;auf &quot; **Seitenlayout**&quot;.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicken Sie neben dem Lead-Layout auf **Bearbeiten** .

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicken Sie auf und ziehen Sie einen neuen **Abschnitt** in das Seitenlayout.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Geben Sie als **Abschnittsnamen** &quot;Markieren&quot;ein und klicken Sie auf **&quot;OK&quot;**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicken Sie auf das Feld **Akquisedatum** und ziehen Sie es in den Abschnitt **Markieren** .

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Wiederholen Sie den obigen Schritt für die folgenden Felder:

   * Akquise-Programm
   * Akquise-Programm-ID
   * Opt-out
   * Inferated City
   * Vorgestellte Firma
   * Inferiertes Land
   * Großraum
   * Abgeleiteter Telefonbereichscode
   * Postleitzahl
   * Inferierte Staatsregion
   * Interessentenbewertung
   * Ursprünglicher Werber
   * Ursprüngliche Suchmaschine
   * Ursprünglicher Suchbegriff
   * Ursprüngliche Quellinformationen
   * Originalquellentyp

   >[!NOTE]
   >
   >Diese Felder müssen im Seitenlayout vorhanden sein, damit Marketo sie lesen/schreiben kann.

   >[!TIP]
   >
   >Erstellen Sie zwei Spalten für die Felder, indem Sie nach rechts auf der Seite ziehen. Sie können Felder von einer Seite zur anderen verschieben, um die Spaltenlängen auszugleichen.

1. Klicken Sie auf **Speichern** , wenn Sie alle Felder hinzugefügt haben.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Wiederholen Sie alle oben genannten Schritte für das Salesforce- **Kontaktseitenlayout**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Denken Sie daran, auf **Speichern** zu klicken, wenn Sie mit dem **Kontaktseitenlayout** fertig sind.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Vergewissern Sie sich, dass das Feld &quot; **Alltägliches Ereignis** &quot;dem **Seitenlayout** des Ereignisses hinzugefügt wurde.

## Synchronisierungsbenutzer erstellen {#create-sync-user}

Marketo benötigt Anmeldeinformationen für den Zugriff auf Salesforce. Dies ist am besten mit einem dedizierten Benutzer, der mit den unten stehenden Schritten erstellt wurde.

>[!NOTE]
>
>Wenn Ihr Unternehmen keine weiteren Salesforce-Lizenzen besitzt, können Sie einen vorhandenen **Marketing-Benutzer** mit dem **Systemadministrator** -Profil verwenden.

1. Geben Sie in der Navigationsleiste &quot;Benutzer&quot;ein und klicken Sie auf &quot; **Benutzer** &quot;unter &quot;Benutzer **verwalten&quot;**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicken Sie auf **Neuer Benutzer**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Füllen Sie die erforderlichen Felder aus und wählen Sie die **Benutzerlizenz aus: Salesforce**, stellen Sie das **Profil ein: Systemadministrator**, aktivieren Sie **Marketing-Benutzer** und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Vergewissern Sie sich, dass die eingegebene E-Mail-Adresse gültig ist. Sie müssen sich als Synchronisierungsbenutzer anmelden, um das Kennwort zurückzusetzen.

Ausgezeichnet! Jetzt haben Sie ein Konto, mit dem Marketo eine Verbindung zu Salesforce herstellen kann. Machen wir es!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Schritt 3 von 3: Connect Marketing und Salesforce (Professional)](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



