---
description: Berechtigungssatz für Sales Insight hinzufügen - Marketo Docs - Produktdokumentation
title: Berechtigungssatz "Sales Insight"hinzufügen
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 3%

---

# Berechtigungssatz &quot;Sales Insight&quot;hinzufügen {#add-sales-insight-permission-set}

Führen Sie die folgenden Schritte aus, um Zugriff auf Sales Insight-Funktionen in Salesforce hinzuzufügen. Gilt für Salesforce Classic und Lighting

>[!PREREQUISITES]
>
>[Aktualisieren Sie Ihr Sales Insight Salesforce-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} auf Version 1.8000 oder höher, um diese Funktion zu verwenden.

>[!IMPORTANT]
>
>Wenn Sie Sales Insight bisher Zugriff auf alle Profile gewährt und/oder Sales Insight für alle Ihre Benutzer implementiert haben, müssen Sie [den Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}, um diesen Berechtigungssatz zu verwenden.

## Überblick {#overview}

Die Berechtigung &quot;Marketo App&quot;ist Teil des Sales Insight Salesforce -Pakets. Sie umfasst den Zugriff auf die unten genannten Objekte, Apex-Klassen und visualforce-Seiten. Diese sind für den Zugriff auf alle Sales Insight-Funktionen erforderlich.

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
   <td>Best-Bets-Ansichten</td> 
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
   <td>InteressantMomentsCache</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>Marketo Sales Insight-Konfig.</td> 
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
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

* Apex-Klassenzugriff: 159 Apex-Klassen, die mit &quot;mkto_si&quot;beginnen
* Visualforce-Seitenzugriff: 64 Visualforce-Seiten, die mit &quot;mkto_si&quot;beginnen
* Benutzerdefinierte Einstellungsdefinitionen: mkto_si.Marketo-Einstellungen und mkto_si.Benutzereinstellungen

## Hinzufügen von Marketo App-Berechtigungen für Benutzer {#adding-marketo-app-permission-set-to-users}

1. Melden Sie sich bei Ihrem Salesforce-Konto an.

1. Klicken Sie auf **Einrichten**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Klicken Sie unter &quot;Administrator&quot;auf &quot;**Benutzer verwalten**&quot;und dann auf &quot;**Benutzer**&quot;.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Wählen Sie unter &quot;Alle Benutzer&quot;den Benutzer aus, auf den Sie Zugriff gewähren möchten, und klicken Sie dann auf **Zuweisungen von Berechtigungssätzen**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Klicken Sie auf **Zuweisungen bearbeiten**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Wählen Sie **Marketo App Access** aus den verfügbaren Berechtigungssätzen und dann **Add**. Klicken Sie auf **Speichern**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Wenn Sie nun auf der Seite &quot;Benutzerdetails&quot;nach unten scrollen, sehen Sie &quot;Marketo App-Zugriff&quot;unter &quot;Zuweisungen von Berechtigungssätzen&quot;.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Benutzer ohne Zugriff auf Sales Insight erhalten folgende Meldung: &quot;Sie verfügen nicht über ausreichende Berechtigungen für den Zugriff auf diese Registerkarte.&quot;

Das ist alles! Sie haben erfolgreich Sales Insight-Zugriff hinzugefügt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, für das Sie Zugriff hinzufügen möchten.
