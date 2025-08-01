---
unique-page-id: 2360364
description: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited) - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 3%

---

# Schritt 2 von 3: Erstellen eines [!DNL Salesforce] für Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Diese Schritte müssen von einem [!DNL Salesforce] Administrator durchgeführt werden

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder hinzufügen zu [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In diesem Artikel richten Sie Benutzerberechtigungen in [!DNL Salesforce] Profil ein und erstellen ein Marketo-[!DNL Salesforce] Integrationskonto.

## Profil erstellen {#create-a-profile}

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Geben Sie „Profile“ in die Navigationssuchleiste ein und klicken Sie auf den Link **[!UICONTROL Profile]**.

   ![](assets/sfdc-profiles-hands.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Wählen Sie **[!UICONTROL Standardbenutzer]**, nennen Sie das Profil &quot;Marketo-Salesforce Sync“ und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Festlegen von Profilberechtigungen {#set-profile-permissions}

1. Klicken Sie **[!UICONTROL Bearbeiten]**, um die Sicherheitsberechtigungen festzulegen.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Stellen Sie **[!UICONTROL Abschnitt]** Administratorberechtigungen“ sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * [!UICONTROL API aktiviert]
   * [!UICONTROL Bearbeiten von HTML-Vorlagen]
   * [!UICONTROL Öffentliche Dokumente verwalten]
   * [!UICONTROL Verwalten öffentlicher Vorlagen]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie das Kontrollkästchen **[!UICONTROL Kennwort läuft nie ab]** aktivieren.

1. Stellen Sie [!UICONTROL &#x200B; Abschnitt „Allgemeine Benutzerberechtigungen] sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * [!UICONTROL Leads konvertieren]
   * [!UICONTROL Ereignisse bearbeiten]
   * [!UICONTROL Aufgaben bearbeiten]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Stellen Sie im Abschnitt [!UICONTROL Standardobjektberechtigungen] sicher, dass [!UICONTROL Lesen, Erstellen, Bearbeiten und Löschen] Berechtigungen für Folgendes überprüft werden:

   * [!UICONTROL Konten]
   * [!UICONTROL Kampagnen]
   * [!UICONTROL Kontakte]
   * [!UICONTROL Leads]
   * [!UICONTROL Opportunities]

   >[!NOTE]
   >
   >Gewähren Sie Berechtigungen für [!UICONTROL Kampagnen], wenn Sie die Kampagnensynchronisierung verwenden möchten.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Wenn Sie fertig sind **[!UICONTROL klicken Sie unten]** der Seite auf „Speichern“.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Festlegen von Feldberechtigungen {#set-field-permissions}

1. Besprechen Sie mit Ihren Marketern, um herauszufinden, welche benutzerdefinierten Felder zum Synchronisieren erforderlich sind.

   >[!NOTE]
   >
   >Dieser Schritt verhindert, dass Felder, die Sie nicht benötigen, in Marketo angezeigt werden. Dadurch wird die Anzeige übersichtlicher und die Synchronisierung beschleunigt.

1. Gehen Sie auf der Seite mit den Profildetails zum Abschnitt **[!UICONTROL Sicherheit auf Feldebene]**. Klicken Sie **[!UICONTROL Anzeigen]**, um die Barrierefreiheit für die Objekte zu bearbeiten:

   * [!UICONTROL Lead]
   * [!UICONTROL Kontakt]
   * [!UICONTROL Konto]
   * [!UICONTROL Opportunity]

   >[!TIP]
   >
   >Sie können andere Objekte entsprechend den Anforderungen Ihres Unternehmens konfigurieren.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Klicken Sie für jedes Objekt auf **[!UICONTROL Bearbeiten]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Suchen Sie die nicht benötigten Felder und stellen Sie sicher, dass **[!UICONTROL Lesezugriff]** und **[!UICONTROL Bearbeitungszugriff]** deaktiviert sind. Klicken **[!UICONTROL abschließend]** Speichern“.

   >[!NOTE]
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

   ![](assets/sfdc-sync-field-edit2.png)

1. Nachdem Sie alle nicht benötigten Felder deaktiviert haben, müssen Sie **[!UICONTROL Lesezugriff und Bearbeitungszugriff]** für die folgenden Objektfelder überprüfen. Klicken **[!UICONTROL abschließend]** Speichern“.

<table>
 <tbody>
  <tr>
   <th>Objekt</th>
   <th>Felder</th>
  </tr>
  <tr>
   <td>Konto</td>
   <td>Feld eingeben</td>
  </tr>
  <tr>
   <td>Ereignis</td>
   <td>Alle Felder</td>
  </tr>
  <tr>
   <td>Aufgabe</td>
   <td>Alle Felder</td>
  </tr>
 </tbody>
</table>

![](assets/sfdc-check-the-boxes.png)

## Synchronisierungskonto für Marketo-Salesforce erstellen {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Erstellen Sie ein dediziertes [!DNL Salesforce] (z. B. marketo@yourcompany.com), um die von Marketo vorgenommenen Änderungen von denen anderer [!DNL Salesforce] zu unterscheiden.

1. Geben Sie in die Navigationssuchleiste „Benutzer verwalten“ ein und klicken Sie dann auf **[!UICONTROL Benutzer]**. Klicken Sie auf **[!UICONTROL Neuer Benutzer]**.

   ![](assets/sfdc-new-users.png)

1. Füllen Sie die erforderlichen Felder aus. Wählen Sie dann die **[!UICONTROL Benutzerlizenz: Salesforce]** und das zuvor erstellte Profil aus. Klicken **[!UICONTROL abschließend]** Speichern“.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Schritt 2 von 3 ist abgeschlossen.

>[!NOTE]
>
>[Schritt 3 von 3: Marketo verbinden und [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
