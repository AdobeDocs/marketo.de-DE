---
unique-page-id: 2360364
description: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketing (Enterprise/Unlimited - Marketing Docs - Produktdokumentation
title: Schritt 2 von 3 - Erstellen eines Salesforce-Benutzers für Marketing (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator ausgeführt werden

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: hinzufügen Marketo-Felder an Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

>



In diesem Artikel richten Sie Benutzerberechtigungen im Salesforce-Profil ein und erstellen ein Marketing-Salesforce-Integrationskonto.

## Profil {#create-a-profile} erstellen

1. Klicken Sie auf **Setup**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Geben Sie &quot;Profile&quot;in die Navigationsleiste ein und klicken Sie auf den Link **Profil**.

   ![](assets/sfdc-profiles-hands.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Wählen Sie **Standardbenutzer**, geben Sie dem Profil den Namen &quot;Marketing-Salesforce-Synchronisierung&quot;und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Festlegen von Profil-Berechtigungen {#set-profile-permissions}

1. Klicken Sie auf **Bearbeiten**, um die Sicherheitsberechtigungen festzulegen.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Vergewissern Sie sich, dass unter dem Abschnitt **Administrative Berechtigungen** die folgenden Kontrollkästchen aktiviert sind:

   * API aktiviert
   * HTML-Vorlagen bearbeiten
   * Öffentliche Dokumente verwalten
   * Öffentliche Vorlagen verwalten

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie das Feld **Kennwort läuft nie ab** markieren.

1. Stellen Sie im Abschnitt &quot;Allgemeine Benutzerberechtigungen&quot;sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * Interessenten konvertieren
   * Ereignisse bearbeiten
   * Aufgaben bearbeiten

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Stellen Sie im Abschnitt &quot;Objektberechtigungen&quot;sicher, dass die Berechtigungen &quot;Lesen&quot;, &quot;Erstellen&quot;, &quot;Bearbeiten&quot;und &quot;Löschen&quot;für Folgendes aktiviert sind:

   * Konten
   * Kampagnen
   * Kontakte
   * Interessenten
   * Chancen

   >[!NOTE]
   >
   >Erteilen Sie Berechtigungen für die Kampagnen, wenn Sie die Kampagne-Synchronisierung verwenden möchten.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Klicken Sie abschließend unten auf der Seite auf **Speichern**.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Feldberechtigungen festlegen {#set-field-permissions}

1. Sprechen Sie mit Ihren Marketingexperten, um herauszufinden, welche benutzerdefinierten Felder synchronisiert werden müssen.

   >[!NOTE]
   >
   >Dieser Schritt verhindert, dass nicht benötigte Felder in Marketo angezeigt werden, was die Übersichtlichkeit reduziert und die Synchronisierung beschleunigt.

1. Gehen Sie auf der Detailseite zum Profil zu **Sicherheit auf Feldebene**. Klicken Sie auf **Ansicht**, um die Barrierefreiheit für die Objekte zu bearbeiten:

   * `Lead`
   * `Contact`
   * `Account`
   * `Opportunity`

   >[!TIP]
   >
   >Sie können andere Objekte entsprechend den Anforderungen Ihres Unternehmens konfigurieren.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Klicken Sie für jedes Objekt auf **Bearbeiten**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Suchen Sie die nicht benötigten Felder, stellen Sie sicher, dass die Kontrollkästchen **Zugriff lesen **und** Zugriff bearbeiten **deaktiviert sind. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

   ![](assets/sfdc-sync-field-edit2.png)

1. Nachdem Sie alle nicht benötigten Felder deaktiviert haben, müssen Sie für die folgenden Objektfelder die Option **Zugriff lesen und Zugriff bearbeiten **aktivieren. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Objekt</p></th> 
   <th colspan="1" rowspan="1"><p>Felder</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Konto</p></td> 
   <td colspan="1" rowspan="1"><p>Feld Typ</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ereignis</p></td> 
   <td colspan="1" rowspan="1"><p>Alle Felder</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Aufgabe</p></td> 
   <td colspan="1" rowspan="1"><p>Alle Felder</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Erstellen Sie ein Marketing-Salesforce-Synchronisierungskonto {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Erstellen Sie ein dediziertes Salesforce-Konto (z. [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#89e4e8fbe2ecfde6c9f0e6fcfbeae6e4f9e8e7f0a7eae6e4)), um die von Marketo vorgenommenen Änderungen im Vergleich zu anderen Salesforce-Benutzern zu unterscheiden.

1. Geben Sie &quot;Benutzer verwalten&quot;in die Navigationsleiste ein und klicken Sie dann auf **Benutzer**. Klicken Sie auf **Neuer Benutzer**.

   ![](assets/sfdc-new-users.png)

1. Füllen Sie die erforderlichen Felder aus. Wählen Sie dann die **Benutzerlizenz: Salesforce** und das zuvor erstellte Profil. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Schritt 2 von 2 ist abgeschlossen.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Schritt 3 von 3: Connect Marketing und Salesforce (Enterprise/Unlimited)](step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)

>



