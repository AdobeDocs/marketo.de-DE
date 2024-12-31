---
description: Zugriff auf Sales Insights entfernen - Marketo-Dokumente - Produktdokumentation
title: Zugriff auf Sales Insights entfernen
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 6%

---

# Zugriff auf Sales Insights entfernen {#remove-sales-insight-access}

Gehen Sie wie folgt vor, um den Zugriff auf Sales Insight-Funktionen in Salesforce zu entfernen. Gilt für Salesforce Classic und Lightning.

## Überblick {#overview}

Für den Zugriff auf alle Sales Insight-Funktionen ist eine Berechtigung für die unten genannten Objekte, Apex-Klassen und VisualForce-Seiten erforderlich. Wenn Sie diese entfernen, wird der Zugriff auf Sales Insights entfernt.

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

## Entfernen des Zugriffs auf Sales Insight {#removing-access-to-sales-insight}

1. Melden Sie sich bei Ihrem Salesforce-Konto an.

1. Klicken Sie **Setup**.

   ![](assets/remove-sales-insight-access-1.png)

1. Klicken Sie unter „Administrator **auf** Benutzer verwalten **und dann auf**.

1. Klicken Sie auf das Profil, das Sie aktualisieren möchten, und dann auf **Bearbeiten**.

1. Scrollen Sie unter Registerkarteneinstellungen nach unten zu „Benutzerdefinierte Registerkarteneinstellungen“.

1. Wählen Sie die Option „Tab Hidden“ aus der Dropdown-Liste für Marketo Sales Insight Config und MSI Marketo Sales Outbox.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scrollen Sie nach unten zu „Benutzerdefinierte Objektberechtigungen“.

1. Entfernen Sie den Zugriff „Lesen, Erstellen, Bearbeiten, Löschen“ aus folgenden Objekten:

   * BestBetsCache
   * Details zur Ansicht mit vielversprechenden Kontakten
   * Beste Ansichten
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Marketo Sales Insight-Konfig.
   * Scoring-Cache
   * Werte
   * WebActivityCache

1. Scrollen Sie nach unten zum Abschnitt „Aktivierter Apex-Klassenzugriff“. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie im Abschnitt „Aktivierte Apex-Klassen“ alle Klassen aus, die mit „mkto_si“ beginnen. Dies sollte bis zu 159 Klassen umfassen.

1. Klicken Sie **Entfernen** und dann **Speichern**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scrollen Sie nach unten zum Abschnitt „Seitenzugriff erzwingen“. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie im Abschnitt „Aktivierte VisualForce-Seiten“ alle Seiten aus, die mit „mkto_si“ beginnen. Dadurch sollten bis zu 64 Seiten hinzugefügt werden.

1. Klicken Sie **Entfernen** und dann **Speichern**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scrollen Sie nach unten zum Abschnitt „Zugriff auf benutzerdefinierte Einstellungsdefinitionen aktiviert“. Klicken Sie auf **Bearbeiten**.

1. Wählen Sie &quot;Marketo Sales Insight.mkto_si.Marketo Settings“ und &quot;Marketo Sales Insight.mkto_si.User Preferences“ aus.

1. Klicken Sie **Entfernen** und dann **Speichern**.

   ![](assets/remove-sales-insight-access-6.png)

Das ist alles! Sie haben den Zugriff auf Sales Insight erfolgreich entfernt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, dem Sie den Zugriff entziehen möchten.
