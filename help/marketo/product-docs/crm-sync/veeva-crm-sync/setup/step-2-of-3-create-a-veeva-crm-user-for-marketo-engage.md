---
description: 'Schritt 2 von 3: Erstellen eines Veeva CRM-Benutzers für Marketo Engage - Marketo-Dokumente - Produktdokumentation'
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
>Die Schritte in diesem Artikel müssen von einem Veeva CRM-Administrator durchgeführt werden.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder zu Salesforce (Professional) hinzufügen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

In diesem Artikel passen Sie Feldberechtigungen mit einem Veeva CRM-Seitenlayout an und erstellen einen Marketo-Veeva CRM-Synchronisierungsbenutzer.

## Festlegen von Seiten-Layouts {#set-page-layouts}

Mit diesen Schritten kann der Marketo-Synchronisierungsbenutzer die benutzerdefinierten Felder aktualisieren.

1. Klicken Sie auf die Seitenlayouts Konto (Personenkonto) in der Navigationssuchleiste, ohne die Eingabetaste zu drücken, und klicken Sie auf **[!UICONTROL Seitenlayout]** unter Kontakte.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Klicken Sie auf **[!UICONTROL Seiten-Layouts]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Klicken Sie **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Klicken Sie auf und ziehen Sie einen neuen **[!UICONTROL Abschnitt]** in das Seitenlayout.

1. Geben Sie als Abschnittsnamen &quot;Marketo&quot; ein und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Klicken Sie auf das Feld Bewertung und ziehen Sie es in den Abschnitt Marketo .

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
   >Diese Felder müssen sich im Seiten-Layout befinden, damit Marketo sie lesen/schreiben kann.

   >[!TIP]
   >
   >Erstellen Sie zwei Spalten für die Felder, indem Sie sie nach unten auf die rechte Seite ziehen. Sie können Felder von einer Seite auf die andere verschieben, um die Spaltenlängen auszugleichen.

1. Wenn Sie mit dem HCP-Professional-Layout fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Wiederholen Sie dies für andere Seiten-Layouts des Kontos.

## Profil erstellen {#create-a-profile}

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Geben Sie in die Navigationssuchleiste „Profile“ ein und klicken Sie auf den **[!UICONTROL Profile]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Wählen Sie Standardbenutzer, benennen Sie das Profil &quot;Marketo-Salesforce Sync“ und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Festlegen von Profilberechtigungen {#set-profile-permissions}

1. Klicken Sie **[!UICONTROL Bearbeiten]**, um die Sicherheitsberechtigungen festzulegen.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Stellen Sie im Abschnitt Administratorberechtigungen sicher, dass **[!UICONTROL API aktiviert]** ausgewählt ist.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie das Kontrollkästchen „Kennwort läuft nie ab“ aktivieren.

1. Stellen Sie sicher, dass im Abschnitt Allgemeine Benutzerberechtigungen **[!UICONTROL Ereignisse bearbeiten]** und **[!UICONTROL Aufgaben bearbeiten]** ausgewählt sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Stellen Sie sicher, dass im Abschnitt Standardobjektberechtigungen die Berechtigungen **[!UICONTROL Lesen]**, **[!UICONTROL Erstellen]**, **[!UICONTROL Bearbeiten]** und **[!UICONTROL Löschen]** für Konten und Kontakte überprüft werden.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Stellen Sie im Abschnitt Benutzerdefinierte Objektberechtigungen sicher, dass Leserechte für **[!UICONTROL Aufruf]**, **[!UICONTROL Aufrufschlüsselmeldung]** und alle anderen gewünschten benutzerdefinierten Objekte aktiviert sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Wenn Sie fertig sind **[!UICONTROL klicken Sie unten]** der Seite auf „Speichern“.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Festlegen von Feldberechtigungen {#set-field-permissions}

1. Besprechen Sie mit Ihren Marketern, um herauszufinden, welche benutzerdefinierten Felder zum Synchronisieren erforderlich sind.

   >[!NOTE]
   >
   >Dieser Schritt verhindert, dass Felder, die Sie nicht benötigen, in Marketo angezeigt werden. Dadurch wird die Anzeige übersichtlicher und die Synchronisierung beschleunigt.

1. Gehen Sie auf der Seite mit den Profildetails zum Abschnitt [!UICONTROL Sicherheit auf Feldebene]. Klicken Sie **[!UICONTROL Anzeigen]**, um die Barrierefreiheit für die Objekte „Kontakt“ und „Konto“ zu bearbeiten.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Sie können andere Objekte entsprechend den Anforderungen Ihres Unternehmens konfigurieren.

1. Klicken Sie für jedes Objekt auf **[!UICONTROL Bearbeiten]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Suchen Sie die unnötigen Felder und stellen Sie sicher, dass „Lesezugriff“ und „Bearbeitungszugriff“ _sind_. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

1. Nachdem Sie alle unnötigen Felder deaktiviert haben, aktivieren Sie Lesezugriff und Bearbeitungszugriff für die folgenden Objektfelder. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

<table>
 <tbody>
  <tr>
   <th>Objekt
   <th>Felder
  </tr>
  <tr>
   <td>Konto</td>
   <td>Feld eingeben</td>
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

Marketo benötigt Anmeldeinformationen, um auf Veeva CRM zuzugreifen. Dies geschieht am besten mit einem dedizierten Benutzer, der mit den folgenden Schritten erstellt wurde.

>[!NOTE]
>
>Wenn Ihr Unternehmen über keine zusätzlichen Veeva CRM-Lizenzen verfügt, können Sie einen vorhandenen Marketing-Benutzer mit dem Systemadministratorprofil verwenden.

1. Geben Sie in der Navigationssuchleiste „Benutzer“ ein und klicken Sie unter **[!UICONTROL verwalten]** Benutzer“.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Klicken Sie auf **[!UICONTROL Neuer Benutzer]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Füllen Sie die erforderlichen Felder aus, wählen Sie die Benutzerlizenz: Salesforce aus, legen Sie das Profil: Marketo Sync User fest und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Stellen Sie sicher, dass die eingegebene E-Mail-Adresse gültig ist. Sie müssen sich als Synchronisierungsbenutzer anmelden, um das Kennwort zurückzusetzen.

Ausgezeichnet! Jetzt haben Sie ein Konto, mit dem Marketo Engage eine Verbindung zu Veeva CRM herstellen kann. Lass es uns machen.

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Marketo und Veeva CRM verbinden](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
