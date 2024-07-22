---
description: Entfernen von Sales Insight Access - Marketo Docs - Produktdokumentation
title: Entfernen von Sales Insight Access
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 4%

---

# Entfernen von Sales Insight Access {#remove-sales-insight-access}

Führen Sie die folgenden Schritte aus, um den Zugriff auf Sales Insight-Funktionen in Salesforce zu entfernen. Gilt für Salesforce Classic und Lightning.

## Überblick {#overview}

Für den Zugriff auf alle Sales Insight-Funktionen ist eine Berechtigung für die unten genannten Objekte, Apex-Klassen und visualforce-Seiten erforderlich. Wenn Sie diese entfernen, wird der Zugriff auf Sales Insight entfernt.

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

## Entfernen des Zugriffs auf Sales Insight {#removing-access-to-sales-insight}

1. Melden Sie sich bei Ihrem Salesforce-Konto an.

1. Klicken Sie auf **Einrichten**.

   ![](assets/remove-sales-insight-access-1.png)

1. Klicken Sie unter &quot;Administrator&quot;auf **Benutzer verwalten** und dann auf **Profile**.

1. Klicken Sie auf das Profil, das Sie aktualisieren möchten, und dann auf **Bearbeiten**.

1. Scrollen Sie nach unten zu &quot;Benutzerdefinierte Registerkarteneinstellungen&quot;unter &quot;Registerkarteneinstellungen&quot;.

1. Wählen Sie die Option &quot;Tab ausgeblendet&quot;aus der Dropdown-Liste für Marketo Sales Insight Config und MSI Marketo Sales Outbox aus.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scrollen Sie nach unten zu &quot;Benutzerdefinierte Objektberechtigungen&quot;.

1. Entfernen Sie den Zugriff &quot;Lesen, Erstellen, Bearbeiten, Löschen&quot;aus den folgenden Objekten:

   * BestBetsCache
   * Details zur Ansicht mit vielversprechenden Kontakten
   * Best-Bets-Ansichten
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InteressantMomentsCache
   * Marketo Sales Insight-Konfig.
   * ScoringCache
   * Werte
   * WebActivityCache

1. Scrollen Sie nach unten zum Abschnitt &quot;Aktivierter Apex-Klassenzugriff&quot;. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie im Abschnitt &quot;Aktivierte Apex-Klassen&quot;alle Klassen aus, die mit &quot;mkto_si&quot;beginnen. Dies sollte bis zu 159 Klassen ergeben.

1. Klicken Sie auf **Entfernen** und dann auf **Speichern**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scrollen Sie nach unten zum Abschnitt &quot;Aktivierter visueller Seitenzugriff&quot;. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie im Abschnitt &quot;Aktivierte Visualisierungsseiten&quot;alle Seiten aus, die mit &quot;mkto_si&quot;beginnen. Dies sollte bis zu 64 Seiten umfassen.

1. Klicken Sie auf **Entfernen** und dann auf **Speichern**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scrollen Sie nach unten zum Abschnitt &quot;Zugriff auf aktivierte benutzerdefinierte Einstellungen - Zugriff&quot;. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot;und &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Klicken Sie auf **Entfernen** und dann auf **Speichern**.

   ![](assets/remove-sales-insight-access-6.png)

Das ist alles! Sie haben den Zugriff auf Sales Insight erfolgreich entfernt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, für das Sie den Zugriff entfernen möchten.
