---
description: 'Schritt 2 von 3: Erstellen eines VEC CRM-Benutzers für Marketo Engage - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Erstellen eines Veeva CRM-Benutzers für Marketo Engage'
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 6%

---

# Schritt 2 von 3: Erstellen eines Veeva CRM-Benutzers für Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>Die Schritte in diesem Artikel müssen von einem Veeva CRM-Administrator ausgeführt werden.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

In diesem Artikel passen Sie die Feldberechtigungen mit einem VEE CRM-Seitenlayout an und erstellen einen Marketo-VEE CRM-Synchronisierungsbenutzer.

## Festlegen von Seitenlayouts {#set-page-layouts}

Mit diesen Schritten kann der Benutzer für die Marketo-Synchronisierung die benutzerdefinierten Felder aktualisieren.

1. Klicken Sie in der Navigationssuchleiste auf die Layouts der Seite Konto (Benutzerkonto), ohne die Eingabetaste zu drücken, und klicken Sie unter Kontakte auf **[!UICONTROL Seitenlayout]** .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Klicken Sie auf **[!UICONTROL Seiten-Layouts]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Klicken Sie auf **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Klicken Sie auf einen neuen Abschnitt **[!UICONTROL Abschnitt]** und ziehen Sie ihn in das Seitenlayout.

1. Geben Sie &quot;Marketo&quot;als Abschnittsnamen ein und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Klicken Sie auf das Feld Punktzahl und ziehen Sie es in den Bereich Marketo .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Wiederholen Sie den obigen Schritt für die folgenden Felder:

   * Abgeleiteter Ort
   * Abgeleitetes Unternehmen
   * Abgeleitetes Land
   * Abgeleiteter Stadtbereich
   * Abgeleitete Vorwahl
   * Abgeleitete Postleitzahl
   * Abgeleitetes Bundesland/abgeleitete Region

   >[!NOTE]
   >
   >Diese Felder müssen im Seitenlayout vorhanden sein, damit Marketo sie lesen/schreiben kann.

   >[!TIP]
   >
   >Erstellen Sie zwei Spalten für die Felder, indem Sie sie nach rechts auf der Seite ziehen. Sie können Felder von einer Seite zur anderen verschieben, um die Spaltenlängen auszugleichen.

1. Wenn Sie mit dem HCP-Professional-Layout fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Wiederholen Sie diesen Vorgang für andere Kontoseitenlayouts.

## Profil erstellen {#create-a-profile}

1. Klicken Sie auf **[!UICONTROL Einrichten]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Geben Sie &quot;profiles&quot;in die Navigationssuchleiste ein und klicken Sie auf den Link **[!UICONTROL Profile]** .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Wählen Sie Standardbenutzer aus, geben Sie dem Profil den Namen &quot;Marketo-Salesforce Sync&quot;und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Profilberechtigungen festlegen {#set-profile-permissions}

1. Klicken Sie auf **[!UICONTROL Bearbeiten]** , um die Sicherheitsberechtigungen festzulegen.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Vergewissern Sie sich, dass im Abschnitt &quot;Administratorberechtigungen&quot;die Option **[!UICONTROL API aktiviert]** ausgewählt ist.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie das Kontrollkästchen Kennwort läuft nie ab aktivieren.

1. Stellen Sie im Abschnitt &quot;Allgemeine Benutzerberechtigungen&quot;sicher, dass **[!UICONTROL Ereignisse bearbeiten]** und **[!UICONTROL Aufgaben bearbeiten]** ausgewählt sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Stellen Sie im Abschnitt &quot;Standardobjektberechtigungen&quot;sicher, dass die Berechtigungen **[!UICONTROL Gelesen]**, **[!UICONTROL Erstellen]**, **[!UICONTROL Bearbeiten]** und **[!UICONTROL Löschen]** für Konten und Kontakte aktiviert sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Stellen Sie im Abschnitt &quot;Berechtigungen für benutzerdefinierte Objekte&quot;sicher, dass die Leseberechtigungen für **[!UICONTROL Aufruf]**, **[!UICONTROL Schlüsselmeldung aufrufen]** und alle anderen gewünschten benutzerdefinierten Objekte aktiviert sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Klicken Sie abschließend unten auf der Seite auf **[!UICONTROL Speichern]** .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Feldberechtigungen festlegen {#set-field-permissions}

1. Diskutieren Sie mit Ihren Marketingexperten, um herauszufinden, welche benutzerdefinierten Felder synchronisiert werden müssen.

   >[!NOTE]
   >
   >Dadurch wird verhindert, dass nicht benötigte Felder in Marketo angezeigt werden, was die Übersichtlichkeit verringert und die Synchronisierung beschleunigt.

1. Wechseln Sie auf der Seite mit den Profildetails zum Abschnitt [!UICONTROL Sicherheit auf Feldebene ] . Klicken Sie auf **[!UICONTROL Anzeigen]** , um die Barrierefreiheit für die Objekte Kontakt und Konto zu bearbeiten.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Sie können entsprechend den Anforderungen Ihres Unternehmens weitere Objekte konfigurieren.

1. Klicken Sie für jedes Objekt auf **[!UICONTROL Bearbeiten]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Suchen Sie die unnötigen Felder und stellen Sie sicher, dass &quot;Lesezugriff&quot;und &quot;Zugriff bearbeiten&quot;_deaktiviert_ sind. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

1. Nachdem Sie alle unnötigen Felder deaktiviert haben, aktivieren Sie die Option Zugriff lesen und Zugriff bearbeiten für die folgenden Objektfelder. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

<table>
 <tbody>
  <tr>
   <th>Objekt
   <th>Felder
  </tr>
  <tr>
   <td>Konto</td>
   <td>Feld Typ</td>
  </tr>
  <tr>
   <td>Veranstaltung</td>
   <td>Alle Felder</td>
  </tr>
  <tr>
   <td>Aufgabe</td>
   <td>Alle Felder</td>
  </tr>
 </tbody>
</table>

## Synchronisierungsbenutzer erstellen {#create-sync-user}

Marketo benötigt Anmeldeinformationen für den Zugriff auf Veeva CRM. Dies sollte am besten mit einem dedizierten Benutzer durchgeführt werden, der mit den folgenden Schritten erstellt wurde.

>[!NOTE]
>
>Wenn Ihr Unternehmen über keine zusätzlichen VEC CRM-Lizenzen verfügt, können Sie einen vorhandenen Marketing-Benutzer mit dem Profil &quot;Systemadministrator&quot;verwenden.

1. Geben Sie &quot;Benutzer&quot;in die Navigationssuchleiste ein und klicken Sie unter &quot;Benutzer verwalten&quot;auf **[!UICONTROL Benutzer]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Klicken Sie auf **[!UICONTROL Neuer Benutzer]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Füllen Sie die erforderlichen Felder aus, wählen Sie die Anwenderlizenz: Salesforce, legen Sie das Profil: Marketo Sync User fest und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Vergewissern Sie sich, dass die von Ihnen eingegebene E-Mail-Adresse gültig ist. Sie müssen sich als Synchronisierungsbenutzer anmelden, um das Kennwort zurückzusetzen.

Ausgezeichnet! Jetzt haben Sie ein Konto, über das Marketo Engage eine Verbindung mit dem Vevar-CRM herstellen kann. Machen wir es!

>[!MORELIKETHIS]
>
>[Schritt 3 vom 3: Verbinden von Marketo und Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
