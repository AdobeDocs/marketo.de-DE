---
unique-page-id: 2360364
description: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 4%

---

# Schritt 2 von 3: Salesforce-Benutzer für Marketo erstellen (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Diese Schritte müssen von einem Salesforce-Administrator ausgeführt werden

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In diesem Artikel richten Sie Benutzerberechtigungen im Salesforce-Profil ein und erstellen ein Marketo-Salesforce-Integrationskonto.

## Erstellen eines Profils {#create-a-profile}

1. Klicken **Einrichtung**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Geben Sie &quot;profiles&quot;in die Navigationssuchleiste ein und klicken Sie auf **Profile** Link.

   ![](assets/sfdc-profiles-hands.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Auswählen **Standardbenutzer**, benennen Sie das Profil &quot;Marketo-Salesforce Sync&quot;und klicken Sie auf **Speichern**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Profilberechtigungen festlegen {#set-profile-permissions}

1. Klicken **Bearbeiten** , um die Sicherheitsberechtigungen festzulegen.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Unter dem **Administratorberechtigungen** müssen Sie sicherstellen, dass die folgenden Kästchen aktiviert sind:

   * API aktiviert
   * HTML-Vorlagen bearbeiten
   * Öffentliche Dokumente verwalten
   * Verwalten öffentlicher Vorlagen

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Überprüfen Sie unbedingt die **Kennwort läuft nie ab** ankreuzen.

1. Stellen Sie im Abschnitt &quot;Allgemeine Benutzerberechtigungen&quot;sicher, dass die folgenden Kontrollkästchen aktiviert sind:

   * Leads konvertieren
   * Ereignisse bearbeiten
   * Aufgaben bearbeiten

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Stellen Sie im Abschnitt &quot;Standardobjektberechtigungen&quot;sicher, dass die Berechtigungen &quot;Lesen&quot;, &quot;Erstellen&quot;, &quot;Bearbeiten&quot;und &quot;Löschen&quot;für Folgendes aktiviert sind:

   * Konten
   * Kampagnen
   * Kontakte
   * Leads
   * Opportunities

   >[!NOTE]
   >
   >Gewähren Sie den Kampagnen Berechtigungen, wenn Sie die Kampagnensynchronisierung verwenden möchten.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Klicken Sie abschließend auf **Speichern** unten auf der Seite.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Feldberechtigungen festlegen {#set-field-permissions}

1. Diskutieren Sie mit Ihren Marketingexperten, um herauszufinden, welche benutzerdefinierten Felder synchronisiert werden müssen.

   >[!NOTE]
   >
   >Dadurch wird verhindert, dass nicht benötigte Felder in Marketo angezeigt werden, was die Übersichtlichkeit verringert und die Synchronisierung beschleunigt.

1. Gehen Sie auf der Seite mit den Profildetails zu **Sicherheit auf Feldebene** Abschnitt. Klicken **Ansicht** So bearbeiten Sie die Barrierefreiheit für die Objekte:

   * Lead
   * Kontakt
   * Konto
   * Chance

   >[!TIP]
   >
   >Sie können entsprechend den Anforderungen Ihres Unternehmens weitere Objekte konfigurieren.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Klicken Sie für jedes Objekt auf **Bearbeiten**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Suchen Sie die nicht erforderlichen Felder. Stellen Sie sicher, dass **Lesezugriff** und **Zugriff bearbeiten** deaktiviert sind. Klicken **Speichern** wenn Sie fertig sind.

   >[!NOTE]
   >
   >Bearbeiten Sie nur die Barrierefreiheit für die benutzerdefinierten Felder.

   ![](assets/sfdc-sync-field-edit2.png)

1. Nachdem Sie alle nicht erforderlichen Felder deaktiviert haben, müssen Sie die Option **Zugriff lesen und bearbeiten** für die folgenden Objektfelder. Klicken **Speichern** wenn Sie fertig sind.

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
   <td colspan="1" rowspan="1"><p>Veranstaltung</p></td> 
   <td colspan="1" rowspan="1"><p>Alle Felder</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Aufgabe</p></td> 
   <td colspan="1" rowspan="1"><p>Alle Felder</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Marketo-Salesforce-Synchronisierungskonto erstellen {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Erstellen Sie ein dediziertes Salesforce-Konto (z. B. marketo@yourcompany.com), um zwischen den von Marketo vorgenommenen Änderungen und anderen Salesforce-Benutzern zu unterscheiden.

1. Geben Sie &quot;Benutzer verwalten&quot;in die Navigationssuchleiste ein und klicken Sie dann auf **Benutzer**. Klicken Sie auf **Neuer Benutzer**.

   ![](assets/sfdc-new-users.png)

1. Füllen Sie die erforderlichen Felder aus. Wählen Sie anschließend die **Anwenderlizenz: Salesforce** und das zuvor von Ihnen erstellte Profil. Klicken **Speichern** wenn Sie fertig sind.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Schritt 2 von 2 ist abgeschlossen.

>[!NOTE]
>
>[Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
