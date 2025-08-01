---
description: Zugriff auf Sales Insight entfernen - Marketo-Dokumente - Produktdokumentation
title: Zugriff auf Sales Insight entfernen
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%

---

# [!DNL Sales Insight] entfernen {#remove-sales-insight-access}

Führen Sie die folgenden Schritte aus, um den Zugriff auf [!DNL Sales Insight] Funktionen in [!DNL Salesforce] zu entfernen. Gilt für [!DNL Salesforce] Classic und Lightning.

## Überblick {#overview}

Für den Zugriff auf alle [!DNL Sales Insight] Funktionen ist eine Berechtigung für die unten genannten Objekte, Apex-Klassen und VisualForce-Seiten erforderlich. Wenn Sie diese entfernen, wird der Zugriff auf [!DNL Sales Insight] entfernt.

**Objekteinstellungen**

<table>
 <tbody>
 <tr>
   <td>BestBetsCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] Details anzeigen</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] Ansichten</td>
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
   <td>[!DNL Marketo Sales Insight] Konfiguration</td>
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

## Entfernen des Zugriffs auf [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Melden Sie sich bei Ihrem [!DNL Salesforce] an.

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/remove-sales-insight-access-1.png)

1. Klicken [!UICONTROL  unter ] auf **[!UICONTROL Benutzer verwalten]** gefolgt von **[!UICONTROL Profile]**.

1. Klicken Sie auf das Profil, das Sie aktualisieren möchten, und dann auf **[!UICONTROL Bearbeiten]**.

1. Scrollen Sie nach unten zu [!UICONTROL Benutzerdefinierte Registerkarteneinstellungen] unter [!UICONTROL Registerkarteneinstellungen].

1. Wählen Sie die Option [!UICONTROL Tab Hidden] aus der Dropdown-Liste für [!DNL Marketo Sales Insight] Config- und MSI [!DNL Marketo Sales] Outbox aus.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scrollen Sie nach unten zu &quot;[!UICONTROL Benutzerdefinierte Objektberechtigungen].“

1. Entfernen Sie den Zugriff „Lesen, Erstellen, Bearbeiten, Löschen“ aus folgenden Objekten:

   * BestBetsCache
   * [!DNL Best Bets]
   * [!DNL Best Bets]
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * [!DNL Marketo Sales Insight]
   * Scoring-Cache
   * Werte
   * WebActivityCache

1. Scrollen Sie nach unten zum Abschnitt [!UICONTROL Aktivierter Zugriff auf Apex]Klassen“. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Abschnitt [!UICONTROL Aktivierte Apex-Klassen] alle Klassen aus, die mit „mkto_si“ beginnen. Dies sollte bis zu 159 Klassen umfassen.

1. Klicken Sie **[!UICONTROL Entfernen]** und dann **[!UICONTROL Speichern]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scrollen Sie nach unten zum Abschnitt [!UICONTROL Aktivierter VisualForce-Seitenzugriff]. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Abschnitt &quot;[!UICONTROL Aktivierte VisualForce]Seiten“ alle Seiten aus, die mit „mkto_si“ beginnen. Dadurch sollten bis zu 64 Seiten hinzugefügt werden.

1. Klicken Sie **[!UICONTROL Entfernen]** und dann **[!UICONTROL Speichern]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scrollen Sie nach unten zum Abschnitt [!UICONTROL Zugriff auf benutzerdefinierte Einstellungsdefinitionen aktiviert]. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie &quot;Marketo Sales Insight.mkto_si.Marketo Settings“ und &quot;Marketo Sales Insight.mkto_si.User Preferences“ aus.

1. Klicken Sie **[!UICONTROL Entfernen]** und dann **[!UICONTROL Speichern]**.

   ![](assets/remove-sales-insight-access-6.png)

Das ist alles! Sie haben [!DNL Sales Insight] Zugriff erfolgreich entfernt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, dem Sie den Zugriff entziehen möchten.
