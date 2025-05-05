---
description: Synchronisierungsstatus von Salesforce - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisierungsstatus
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 14%

---

# Salesforce-Synchronisierungsstatus {#salesforce-sync-status}

Verwenden Sie das Dashboard Synchronisierungsstatus , um Synchronisierungsstatus als Teil der Synchronisierungsschritte und deren Erfolgsstatus anzuzeigen.

Die Synchronisierungsschritte spiegeln Push- oder Pull-Vorgänge für jeden Objekttyp für das Objektschema und die Daten selbst wider. Statistiken umfassen neue Einträge, Aktualisierungen, Löschvorgänge und fehlgeschlagene Zählungen während der Synchronisierung. Benutzer können nach Datum, Vorgangstyp oder Objekttyp filtern. Das Dashboard „Synchronisationsstatus“ zeigt den Status der Synchronisationszyklen der letzten fünf Tage an.

>[!NOTE]
>
>Administratorberechtigungen erforderlich

## Synchronisierungsstatus anzeigen {#view-sync-status}

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-status-1.png)

1. Klicken [!UICONTROL &#x200B; unter &quot;]Integration“ auf **Salesforce** und dann auf die Registerkarte **[!UICONTROL Synchronisierungsstatus]**.

   ![](assets/salesforce-sync-status-2.png)

Standardmäßig werden Statistiken nach den zuletzt gestarteten Versionen sortiert. Sie können sortieren, indem Sie auf das Symbol Sortieren klicken, und zwar von „Gestartet um“ oder „Beendet um“ (von „Zuletzt verwendet“ zu „Älteste„).

![](assets/salesforce-sync-status-3.png)

## Synchronisierungsstatus filtern {#filter-sync-status}

1. Um die Daten zu filtern, klicken Sie auf das Filtersymbol ganz rechts auf der Seite.

   ![](assets/salesforce-sync-status-4.png)

1. Wählen Sie Ihren Datums- und Zeitbereich aus und klicken Sie dann auf die Dropdown-Listen, um nach [!UICONTROL Objekttyp], [!UICONTROL Vorgangstyp] und/oder [!UICONTROL Statustyp] zu filtern.

   ![](assets/salesforce-sync-status-5.png)

1. Klicken Sie auf **[!UICONTROL Übernehmen]**.

   ![](assets/salesforce-sync-status-6.png)

**OPTIONALER SCHRITT**: Um Synchronisierungsfehler zu exportieren, klicken Sie auf **[!UICONTROL Exportieren]**. Die Daten werden als CSV exportiert.

![](assets/salesforce-sync-status-7.png)

## Statusfelder synchronisieren {#sync-status-fields}

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
   <td colspan="1">Startdatum/-zeit des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Beendet um</td> 
   <td colspan="1">Enddatum/-zeit des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objekt</td> 
   <td colspan="1">Objekttyp</td> 
   <td colspan="1">Kontakt, Person, Aufgabe, Opportunity, Lead, Sonstige wie unten beschrieben</td> 
  </tr>  
  <tr> 
   <td colspan="1">Vorgang</td> 
   <td colspan="1">Vorgangstyp</td> 
   <td colspan="1">Vorgangstypen wie unten beschrieben</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status</td> 
   <td colspan="1">Status des Stapels</td> 
   <td colspan="1">Erfolgreich, fehlgeschlagen, unvollständig, in Bearbeitung, bereinigt*</td> 
  </tr>
  <tr> 
   <td colspan="1">Neu</td> 
   <td colspan="1">Anzahl neuer Datensätze</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Aktualisiert</td> 
   <td colspan="1">Anzahl der aktualisierten Einträge</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Gelöscht</td> 
   <td colspan="1">Anzahl gelöschter Datensätze</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Fehlgeschlagenes Element</td> 
   <td colspan="1">Anzahl an Datensätzen, deren Synchronisierung fehlgeschlagen ist</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Übersprungen</td> 
   <td colspan="1">Anzahl der übersprungenen Datensätze, da es für die Synchronisierung keine Änderungen an den Interessenfeldern gab</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;Daten wurden nach fehlgeschlagenem Synchronisierungsschritt wieder in den vorherigen Integritätsstatus zurückgesetzt.

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
   <td colspan="1">Benutzerdefinierte Objekte</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kampagne</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status des Kampagnenmitgliedes</td> 
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
   <td colspan="1">Gelegenheit Kontaktrolle</td> 
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
   <th>Operationstyp</th>
  </tr> 
  <tr> 
   <td colspan="1">Link mit Programm initialisieren</td> 
   <td colspan="1">Kampagne</td> 
   <td colspan="1">Kampagnen mit Programmen verknüpfen</td> 
   <td colspan="1">Update</td>
  </tr>  
  <tr> 
   <td colspan="1">Gespräche abrufen</td> 
   <td colspan="1">Person (Lead)*</td> 
   <td colspan="1">Pull-Konvertierungsaktionen von SFDC nach Marketo. Einheiten (Zahlen) sind Leads, die in Kontakte konvertieren</td> 
   <td colspan="1">Update, Element fehlgeschlagen oder übersprungen</td>
  </tr> 
  <tr> 
   <td colspan="1">Gelöschte abrufen</td> 
   <td colspan="1">Kontakt, Person (Lead), Opportunity, Kampagne, Kampagnenmitglieder, Opportunity-Kontakt, benutzerdefinierte Objekte, Kampagnen, Kampagnenmitgliedsstatus, Opportunity-Kontaktrolle</td> 
   <td colspan="1">Gelöschte Datensätze von SFDC werden mit Marketo synchronisiert</td> 
   <td colspan="1">Gelöschtes, fehlgeschlagenes oder übersprungenes Element</td>
  </tr>  
  <tr> 
   <td colspan="1">Aktualisierungen abrufen</td> 
   <td colspan="1">Aufgabe, Person (Lead), Personen (Lead)-Warteschlange, Kontakt, Ereignis, Opportunity, Konto, Kontotyp, Kampagnenmitglieder, benutzerdefinierte Objekte, Kampagnen, Kampagnenmitgliedsstatus, Ereignisse, Personenstatus, Opportunity, Kontaktrolle der Opportunity</td> 
   <td colspan="1">Aktualisierungen oder neue Datensätze in SFDC werden mit Marketo synchronisiert, Ereignisse werden als Aktivitäten abgerufen</td> 
   <td colspan="1">Neues, aktualisiertes, fehlgeschlagenes oder übersprungenes Element</td>
  </tr>  
  <tr> 
   <td colspan="1">Neue übertragen</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen</td> 
   <td colspan="1">Aufgaben per Push übertragen (Aktivitäten)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Aktualisierungen übertragen</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen, Person, Kontakt, Kampagnen</td> 
   <td colspan="1">Updates und Löschvorgänge per Push an SFDC übertragen</td> 
   <td colspan="1">Update, Element fehlgeschlagen oder übersprungen</td>
  </tr>  
  <tr> 
   <td colspan="1">Schema synchronisieren</td> 
   <td colspan="1">Kampagnenmitglieder, benutzerdefinierte Objekte, Kampagnen, Kampagnenmitgliedsstatus, Aufgaben, Person, Opportunity, Kontaktrolle Opportunity, Benutzer</td> 
   <td colspan="1">Synchronisiert Metadaten für verschiedene Objekte, um zu entscheiden, welche neuen Felder im nächsten Zyklus synchronisiert werden sollen.</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Mit Programm synchronisieren</td> 
   <td colspan="1">Kampagnen</td> 
   <td colspan="1">Synchronisiert das Marketo-Programm mit SFDC Campaign</td> 
   <td colspan="1">Neu, Aktualisierungen, fehlgeschlagen oder übersprungen</td>
  </tr> 
  <tr> 
   <td colspan="1">Aktivitäten aktualisieren</td> 
   <td colspan="1">Aufgaben</td> 
   <td colspan="1">Aktivitäten aus Salesforce abrufen</td> 
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

&#42;Die Branding-Konfiguration auf Abonnementebene entscheidet über die Bezeichnung - „Lead“ oder „Person“ im Bericht.
