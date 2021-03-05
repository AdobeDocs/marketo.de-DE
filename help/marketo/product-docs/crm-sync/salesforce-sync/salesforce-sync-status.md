---
description: Salesforce-Synchronisierungsstatus - Marketing Docs - Produktdokumentation
title: Salesforce-Synchronisierungsstatus
translation-type: tm+mt
source-git-commit: 98af67caaf485535ba2177aa661a503990e8698d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# Salesforce-Synchronisierungsstatus {#salesforce-sync-status}

Verwenden Sie das Dashboard &quot;Synchronisierungsstatus&quot;, um die Synchronisierungsstatistiken als Teil der Synchronisierungsschritte und des Erfolgsstatus der Ansicht zu verwenden.

Die Synchronisierungsschritte spiegeln die Push- oder Pull-Vorgänge jedes Objekttyps für das Schema und die Daten selbst wider. Statistiken behandeln neue Datensätze, Aktualisierungen, Löschvorgänge und fehlgeschlagene Zählungen während der Synchronisierung. Benutzer können nach Datum, Vorgangsart oder Objekttyp filtern. Das Dashboard &quot;Synchronisierungsstatus&quot;zeigt den Status der Synchronisierungszyklen der letzten fünf Tage an.

>[!NOTE]
>
>Administratorberechtigungen erforderlich

## Synchronisierungsstatus der Ansicht {#view-sync-status}

1. Klicken Sie auf **Admin**.

   ![](assets/salesforce-sync-status-1.png)

1. Klicken Sie unter Integration auf Salesforce und dann auf die Registerkarte Synchronisierungsstatus.

   ![](assets/salesforce-sync-status-2.png)

Standardmäßig werden die Statistiken nach den neuesten Startvorgängen sortiert. Sie können die Sortierung nach &quot;Beginnt am&quot;oder &quot;Beendet am&quot;- vom neuesten zum ältesten - durch Klicken auf das Sortiersymbol durchführen.

![](assets/salesforce-sync-status-3.png)

## Filter-Synchronisierungsstatus {#filter-sync-status}

1. Klicken Sie zum Filtern der Daten auf das Filtersymbol ganz rechts auf der Seite.

   ![](assets/salesforce-sync-status-4.png)

1. Wählen Sie Datum und Zeitraum aus und klicken Sie dann auf die Dropdown-Liste(n), um nach Objekttyp, Vorgangsart und/oder Status-Typ zu filtern.

   ![](assets/salesforce-sync-status-5.png)

1. Klicken Sie auf **Apply**.

   ![](assets/salesforce-sync-status-6.png)

**Optionaler Schritt**: Um Synchronisierungsfehler zu exportieren, klicken Sie auf  **Exportieren**. Die Daten werden als CSV exportiert.

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
   <th>Enum-Werte</th> 
  </tr> 
  <tr> 
   <td colspan="1">Beginnt am</td> 
   <td colspan="1">Datum/Uhrzeit des Beginns des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Beendet am</td> 
   <td colspan="1">Enddatum/Uhrzeit des Synchronisierungszyklus (Zeitzone des Benutzers)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objekt</td> 
   <td colspan="1">Objekttyp</td> 
   <td colspan="1">Kontakt, Person, Aufgabe, Gelegenheit, Interessent, Sonstige, wie unten beschrieben</td> 
  </tr>  
  <tr> 
   <td colspan="1">Vorgang</td> 
   <td colspan="1">Vorgangsart</td> 
   <td colspan="1">Vorgangsarten wie unten</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status</td> 
   <td colspan="1">Status des Stapels</td> 
   <td colspan="1">Erfolgreich, Fehlgeschlagen, Unvollständig, In Bearbeitung, Bereinigt*</td> 
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
   <td colspan="1">Anzahl der gelöschten Datensätze</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Fehlgeschlagenes Element</td> 
   <td colspan="1">Anzahl der Datensätze, deren Synchronisierung fehlgeschlagen ist</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Übersprungen</td> 
   <td colspan="1">Anzahl der ausgelassenen Datensätze, da keine Änderungen an den für die Synchronisierung relevanten Feldern vorgenommen wurden</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*Daten wurden nach einem Fehler bei der Synchronisierung auf den vorherigen Integritätsstatus zurückgesetzt.

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
   <td colspan="1">Mitgliederstatus der Kampagne</td> 
  </tr>
  <tr> 
   <td colspan="1">Kontakt</td> 
  </tr>  
  <tr> 
   <td colspan="1">E-Mail-Vorlage</td> 
  </tr>  
  <tr> 
   <td colspan="1">Ereignis</td> 
  </tr> 
  <tr> 
   <td colspan="1">Person (Interessent)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Chancen</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kontaktrolle bei Chancen</td> 
  </tr>  
  <tr> 
   <td colspan="1">Aufgabe</td> 
  </tr>  
  <tr> 
   <td colspan="1">Benutzer</td> 
  </tr>  
 </tbody> 
</table>

## Vorgangsart {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Vorgangsart</th> 
   <th>Gegen diese Objekte gefunden</th> 
   <th>Bemerkungen</th> 
   <th>Art der Operation</th>
  </tr> 
  <tr> 
   <td colspan="1">Link mit Programm einfügen</td> 
   <td colspan="1">Kampagne</td> 
   <td colspan="1">Verknüpfen von Kampagnen mit Programmen</td> 
   <td colspan="1">Aktualisieren</td>
  </tr>  
  <tr> 
   <td colspan="1">Umrechnungen abziehen</td> 
   <td colspan="1">Person (Interessent)*</td> 
   <td colspan="1">Ziehen Sie Konvertierungsaktionen von SFDC nach Marketo. Einheiten(Nummern) sind Interessenten, die in Kontakte konvertieren</td> 
   <td colspan="1">Aktualisieren, Fehlgeschlagenes Element oder Übersprungen</td>
  </tr> 
  <tr> 
   <td colspan="1">Entfernen</td> 
   <td colspan="1">Kontakt, Person (Interessent), Gelegenheit, Kampagne, Kampagne Mitglieder, Kontaktmöglichkeit, Benutzerspezifische Objekte, Kampagnen, Status des Mitglieds der Kampagne, Kontaktrolle für Chancen</td> 
   <td colspan="1">Gelöschte Aufzeichnungen des SFDC, das mit Marketo synchronisiert wird</td> 
   <td colspan="1">Gelöschte, fehlgeschlagene Elemente oder übersprungene Elemente</td>
  </tr>  
  <tr> 
   <td colspan="1">Aktualisierungen abrufen</td> 
   <td colspan="1">Aufgabe, Person (Interessent), Person (Interessent), Warteschlange, Kontakt, Ereignis, Gelegenheit, Konto, Kontotyp, Kampagne Mitglieder, Benutzerspezifische Objekte, Kampagnen, Mitgliedsstatus der Kampagne, Ereignisse, Personenstand, Chancen, Kontaktrolle Chancen</td> 
   <td colspan="1">Aktualisierungen oder neue Datensätze im SFDC mit Marketo synchronisiert, Ereignisse als Aktivitäten abrufen</td> 
   <td colspan="1">Neues, aktualisiertes, fehlgeschlagenes Element oder übersprungen</td>
  </tr>  
  <tr> 
   <td colspan="1">Push new</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen</td> 
   <td colspan="1">Push-Aufgaben (Aktivitäten)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Push-Updates</td> 
   <td colspan="1">Aufgaben, E-Mail-Vorlagen, Person, Kontakt, Kampagnen</td> 
   <td colspan="1">Übermitteln von Updates an das SFDC und Löschen</td> 
   <td colspan="1">Aktualisieren, Fehlgeschlagenes Element oder Übersprungen</td>
  </tr>  
  <tr> 
   <td colspan="1">Schema synchronisieren</td> 
   <td colspan="1">Kampagnen-Mitglieder, Benutzerspezifische Objekte, Kampagnen, Mitgliedsstatus der Kampagne, Aufgaben, Person, Gelegenheit, Kontaktrolle für Gelegenheiten, Benutzer</td> 
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
   <td colspan="1">Aktivitäten aus Salesforce ziehen</td> 
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

*Die Branding-Konfiguration auf Abonnement-Ebene entscheidet über das Etikett - &quot;Lead&quot; oder &quot;Person&quot; im Bericht.
