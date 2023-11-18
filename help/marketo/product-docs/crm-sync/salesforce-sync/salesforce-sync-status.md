---
description: Salesforce-Synchronisierungsstatus - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisierungsstatus
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 14%

---

# Salesforce-Synchronisierungsstatus {#salesforce-sync-status}

Verwenden Sie das Synchronisierungsstatus-Dashboard, um die Synchronisierungsstatistiken als Teil der Synchronisierungsschritte und des Erfolgsstatus anzuzeigen.

Die Synchronisierungsschritte spiegeln die Push- oder Pull-Vorgänge jedes Objekttyps für das Objektschema und die Daten selbst wider. Statistiken decken neue Datensätze, Aktualisierungen, Löschvorgänge und fehlgeschlagene Zählungen während der Synchronisierung ab. Benutzer können nach Datum, Vorgangstyp oder Objekttyp filtern. Das Synchronisierungsstatus-Dashboard zeigt den Status der Synchronisierungszyklen für die letzten fünf Tage an.

>[!NOTE]
>
>Erforderliche Administratorberechtigungen

## Synchronisierungsstatus anzeigen {#view-sync-status}

1. Klicks **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-status-1.png)

1. under [!UICONTROL Integration]klicken **Salesforce**, dann die **[!UICONTROL Synchronisierungsstatus]** Registerkarte.

   ![](assets/salesforce-sync-status-2.png)

Standardmäßig werden die Statistiken nach den letzten Startvorgängen sortiert. Sie können die Sortierung nach &quot;Gestartet am&quot;oder &quot;Beendet am&quot;(vom letzten zum ältesten) vornehmen, indem Sie auf das Sortiersymbol klicken.

![](assets/salesforce-sync-status-3.png)

## Filtersynchronisierungsstatus {#filter-sync-status}

1. Um die Daten zu filtern, klicken Sie auf das Filtersymbol ganz rechts auf der Seite.

   ![](assets/salesforce-sync-status-4.png)

1. Wählen Sie Datum und Zeitraum aus und klicken Sie dann auf die Dropdown-Liste, nach denen Sie filtern möchten [!UICONTROL Objekttyp], [!UICONTROL Aktionstyp], und/oder [!UICONTROL Statustyp].

   ![](assets/salesforce-sync-status-5.png)

1. Klicks **[!UICONTROL Anwenden]**.

   ![](assets/salesforce-sync-status-6.png)

**OPTIONALER SCHRITT**: Um Synchronisierungsfehler zu exportieren, klicken Sie auf **[!UICONTROL Export]**. Die Daten werden als CSV exportiert.

![](assets/salesforce-sync-status-7.png)

## Synchronisierungsstatusfelder {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Feld</th> 
   <th>Beschreibung</th> 
   <th>Aufzählungswerte</th> 
  </tr> 
  <tr> 
   <td colspan="1">Gestartet um</td> 
   <td colspan="1">Datum/Uhrzeit des Starts des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Beendet um</td> 
   <td colspan="1">Enddatum/Endzeit des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objekt</td> 
   <td colspan="1">Objekttyp</td> 
   <td colspan="1">Kontakt, Person, Aufgabe, Chancen, Leiter/innen wie unten beschrieben</td> 
  </tr>  
  <tr> 
   <td colspan="1">Vorgang</td> 
   <td colspan="1">Vorgangstyp</td> 
   <td colspan="1">Aktionstypen wie folgt</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status</td> 
   <td colspan="1">Status des Batches</td> 
   <td colspan="1">Erfolgreich, fehlgeschlagen, nicht abgeschlossen, in Verarbeitung, bereinigt*</td> 
  </tr>
  <tr> 
   <td colspan="1">Neu</td> 
   <td colspan="1">Anzahl neuer Datensätze</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Aktualisiert</td> 
   <td colspan="1">Anzahl der aktualisierten Datensätze</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Gelöscht</td> 
   <td colspan="1">Anzahl gelöschter Datensätze</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Fehlgeschlagenes Element</td> 
   <td colspan="1">Anzahl der Datensätze, deren Synchronisierung fehlgeschlagen ist</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Übersprungen</td> 
   <td colspan="1">Anzahl der übersprungenen Datensätze, da keine Änderungen an den für die Synchronisierung relevanten Feldern vorgenommen wurden</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;Nach einem Synchronisierungsschritt wurden die Daten wieder in den vorherigen Integritätsstatus versetzt.

## Objekttyp {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">Konto</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kontotyp</td> 
  </tr> 
  <tr> 
   <td colspan="1">benutzerdefinierte -Objekte</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kampagne</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kampagnenmitglied Status</td> 
  </tr>
  <tr> 
   <td colspan="1">Kontakt</td> 
  </tr>  
  <tr> 
   <td colspan="1">E-Mail-Vorlage</td> 
  </tr>  
  <tr> 
   <td colspan="1">Veranstaltung</td> 
  </tr> 
  <tr> 
   <td colspan="1">Person (Lead)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Opportunity</td> 
  </tr>  
  <tr> 
   <td colspan="1">Rolle des Opportunity-Kontakts</td> 
  </tr>  
  <tr> 
   <td colspan="1">Aufgabe</td> 
  </tr>  
  <tr> 
   <td colspan="1">Benutzer</td> 
  </tr>  
 </tbody> 
</table>

## Vorgangstyp {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Vorgangstyp</th> 
   <th>Gegen diese Objekte gefunden</th> 
   <th>Bemerkungen</th> 
   <th>Aktionstyp</th>
  </tr> 
  <tr> 
   <td colspan="1">Initlink mit Programm</td> 
   <td colspan="1">Kampagne</td> 
   <td colspan="1">Verknüpfen von Kampagnen mit Programmen</td> 
   <td colspan="1">Aktualisierung</td>
  </tr>  
  <tr> 
   <td colspan="1">Gespräche abrufen</td> 
   <td colspan="1">Person (Lead)*</td> 
   <td colspan="1">Ziehen Sie Konvertierungsaktionen von SFDC nach Marketo. Einheiten (Zahlen) sind Leads, die in Kontakte konvertiert werden</td> 
   <td colspan="1">Aktualisieren, Fehlgeschlagenes Element oder Übersprungen</td>
  </tr> 
  <tr> 
   <td colspan="1">Gelöschte abrufen</td> 
   <td colspan="1">Kontakt, Person (Lead), Gelegenheit, Kampagne, Campaign, Campaign-Mitglieder, Opportunity Contact, Custom Objects, Campaigns, Campaign Member Status, Opportunity Contact Rolle</td> 
   <td colspan="1">Gelöschte Einträge von SFDC, die mit Marketo synchronisiert werden</td> 
   <td colspan="1">Gelöschte, fehlgeschlagene Elemente oder übersprungene Elemente</td>
  </tr>  
  <tr> 
   <td colspan="1">Aktualisierungen abrufen</td> 
   <td colspan="1">Aufgabe, Person (Lead), Personen (Lead)-Warteschlange, Kontakt, Ereignis, Gelegenheit, Konto, Kontotyp, Kampagnenmitglieder, benutzerdefinierte Objekte, Kampagnen, Kampagnenmitgliedschaft, Ereignisse, Personenstand, Chancen, Kontaktrolle für Chancen</td> 
   <td colspan="1">Aktualisierungen oder neue Einträge in SFDC, die mit Marketo synchronisiert werden, Pull-Ereignisse als Aktivitäten</td> 
   <td colspan="1">Neues, aktualisiertes, fehlgeschlagenes Element oder übersprungen</td>
  </tr>  
  <tr> 
   <td colspan="1">Neue übertragen</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen</td> 
   <td colspan="1">Push-Aufgaben (Aktivitäten)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Aktualisierungen übertragen</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen, Person, Kontakt, Kampagnen</td> 
   <td colspan="1">Push von Aktualisierungen an SFDC und auch Löschen</td> 
   <td colspan="1">Aktualisieren, Fehlgeschlagenes Element oder Übersprungen</td>
  </tr>  
  <tr> 
   <td colspan="1">Schema synchronisieren</td> 
   <td colspan="1">Kampagnenmitglieder, benutzerdefinierte Objekte, Kampagnen, Status der Kampagnenmitglieder, Aufgaben, Person, Chancen, Kontaktrolle für Chancen, Benutzer</td> 
   <td colspan="1">Synchronisiert Metadaten für verschiedene Objekte, um zu entscheiden, welche neuen Felder im nächsten Zyklus synchronisiert werden sollen</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Mit Programm synchronisieren</td> 
   <td colspan="1">Kampagnen</td> 
   <td colspan="1">Synchronisiert Marketo-Programm mit SFDC-Kampagnen</td> 
   <td colspan="1">Neu, Updates, Fehlgeschlagen oder Übersprungen</td>
  </tr> 
  <tr> 
   <td colspan="1">Aktivitäten aktualisieren</td> 
   <td colspan="1">Aufgaben</td> 
   <td colspan="1">Pull-Aktivitäten von Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">FKS aktualisieren</td> 
   <td colspan="1">Alle</td> 
   <td colspan="1">Fremdschlüssel aller Objekte aktualisieren</td> 
   <td colspan="1">Nicht zutreffend</td>
  </tr>  
 </tbody> 
</table>

&#42;Die Branding-Konfiguration auf Abonnementebene bestimmt die Bezeichnung &quot;Lead&quot;oder &quot;Person&quot;im Bericht.
