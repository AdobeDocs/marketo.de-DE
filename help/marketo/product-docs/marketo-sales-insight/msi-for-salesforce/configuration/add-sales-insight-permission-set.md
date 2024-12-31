---
description: Hinzufügen des Berechtigungssatzes „Sales Insight“ - Marketo-Dokumente - Produktdokumentation
title: Berechtigungssatz für Sales Insights hinzufügen
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 3%

---

# Berechtigungssatz für Sales Insights hinzufügen {#add-sales-insight-permission-set}

Gehen Sie wie folgt vor, um Zugriff auf Sales Insight-Funktionen in Salesforce hinzuzufügen. Gilt für Salesforce Classic und Lightning

>[!PREREQUISITES]
>
>[Aktualisieren Sie Ihr Sales Insight Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}Paket auf Version 1.8000 oder höher, um diese Funktion zu verwenden.

>[!IMPORTANT]
>
>Wenn Sie zuvor allen Profilen Sales Insights Zugriff erteilt und/oder Sales Insights für alle Ihre Benutzer implementiert haben, müssen Sie [Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} um diesen Berechtigungssatz zu verwenden.

## Überblick {#overview}

Die Berechtigung &quot;Marketo-App“ ist Teil des Sales Insight-Salesforce-Pakets. Dazu gehört der Zugriff auf die unten genannten Objekte, Apex-Klassen und VisualForce-Seiten. Diese sind für den Zugriff auf alle Sales Insight-Funktionen erforderlich.

**Objekteinstellungen**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Details zur Ansicht mit vielversprechenden Kontakten</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Beste Ansichten</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Marketo Sales Insight-Konfig.</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Scoring-Cache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Werte</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
 </tbody> 
</table>

* Apex Class Access: 159 Apex-Klassen, die mit „mkto_si“ beginnen
* VisualForce Seitenzugriff: 64 VisualForce-Seiten, die mit „mkto_si“ beginnen
* Benutzerdefinierte Einstellungsdefinitionen: mkto_si.Marketo Settings &amp; mkto_si.User Preferences

## Hinzufügen des Marketo-App-Berechtigungssatzes zu Benutzenden {#adding-marketo-app-permission-set-to-users}

1. Melden Sie sich bei Ihrem Salesforce-Konto an.

1. Klicken Sie **Setup**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Klicken Sie unter „Administrator“ auf **Benutzer verwalten** und dann auf **Benutzer**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Wählen Sie unter Alle Benutzer den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie dann auf **Zuweisungen für Berechtigungssätze**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Klicken Sie **Zuweisungen bearbeiten**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Wählen Sie **Marketo App Access** aus den verfügbaren Berechtigungssätzen und **Hinzufügen**. Klicken Sie auf **Speichern**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Wenn Sie nun auf der Seite Benutzerdetails nach unten scrollen, sehen Sie „Zugriff auf Marketo-Mobile-Apps“ unter „Zuweisungen von Berechtigungssätzen“.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Benutzende, die keinen Zugriff auf Sales Insight haben, sehen die Meldung: „Sie verfügen nicht über ausreichende Berechtigungen, um auf diese Registerkarte zuzugreifen.“

Das ist alles! Sie haben erfolgreich Sales Insight-Zugriff hinzugefügt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, dem Sie Zugriff hinzufügen möchten.
