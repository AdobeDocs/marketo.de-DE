---
description: Synchronisieren von Anrufen und Aufrufen von Schlüsselmeldungen - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren von Aufrufen und Aufrufen von Schlüsselmeldungen
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 5%

---

# Synchronisieren von Aufrufen und Aufrufen von Schlüsselmeldungen {#syncing-call-and-call-key-messages}

Call and Call Key Message Objects in Veeva CRM werden standardmäßig in Marketo Engage synchronisiert. Marketo synchronisiert Daten, die bis zu 6 Monate alt sind, basierend auf dem Erstellungsdatum des Aufrufs.

>[!NOTE]
>
>Marketo bewahrt die Aufrufdaten bis zu sechs Monate nach dem Datum des Aufrufs auf.

**Welche Trigger/Filter beziehen sich auf die Schlüsselmeldung &quot;Aufruf und Aufruf&quot;?**

Auslöser:

* Zum Aufruf hinzugefügt
* Aus Aufruf entfernt
* Zum Aufruf der Schlüsselmeldung hinzugefügt
* Aus der Schlüsselmeldung &quot;Aufruf&quot; entfernt
* Aktualisierter Aufruf
* Aktualisierte Meldung über den Anrufschlüssel

Filter:

* Hat-Aufruf
* Hat Schlüsselmeldung zum Aufruf

Die folgenden Felder in den Meldungen &quot;Aufruf&quot;und &quot;Schlüssel aufrufen&quot;werden synchronisiert und können als Begrenzungen und Trigger verwendet werden.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Objekt
      </th>
      <th>
        Feldbezeichnung
      </th>
      <th>
        Beschreibung
      </th>
      <th>
        Feldname
      </th>
      <th>
        Datentyp
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Anruf</td>
      <td>Buchhalter</td>
      <td>Sucht nach dem Konto, mit dem der Aufruf verknüpft ist.</td>
      <td>Account_vod_c</td>
      <td>Suche (Konto)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Aufruftyp</td>
      <td>Art des Aufrufs, der basierend auf Typ und Inhalt des Aufrufs systemverwaltet wird. Dieses Feld wird für Berichterstellungszwecke verwendet. Gültige Werte sind: Nur Details, Details mit Beispiel, Gruppendetails, Gruppendetails mit Beispiel, Nur Beispiel. Diese Werte sollten nicht geändert werden, aber die Übersetzungen für diese Picklists können geändert werden. Teilnehmer haben denselben Aufruftyp wie der Header-Aufruf. Bei einem Gruppenaufruf mit 3 Profis weisen alle vier Datensätze den Aufruftyp "Gruppendetails"auf</td>
      <td>Call_Type_vod_c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
     <td>Anruf</td>
      <td>Kontakt</td>
      <td>Suchen Sie nach dem Kontakt (falls vorhanden), mit dem der Aufruf verknüpft ist.</td>
      <td>Contact_vod_c</td>
      <td>Lookup(Contact)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Datum</td>
      <td>Das Datum des Aufrufs, an dem er zum ersten Mal gespeichert oder gesendet wurde. Dieses Feld wird über einen Trigger auf das aktuelle Datum gesetzt, wenn weder das Datums- noch das Datum-Uhrzeit-Feld angegeben ist.</td>
      <td>Call_Date_vod_c</td>
      <td>Datum</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Ist der übergeordnete Aufruf?</td>
      <td>Formelfeld , um zu bestimmen, ob der Aufrufdatensatz der übergeordnete Aufruf oder ein Teilnehmeraufruf-Datensatz ist. 1 zeigt an, dass der Datensatz der übergeordnete Aufruf ist. 0 bedeutet, dass es sich um einen Teilnehmeraufruf handelt.</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>Formel (Zahl)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Status</td>
      <td>Status des Aufrufs: Geplant, gespeichert oder Gesendet. Verwenden Sie die Übersetzungs-Workbench, um die Anzeigewerte zu ändern. Die aufrufenden Trigger sehen sich dieses Feld an, um zu sehen, ob der Aufruf gesperrt (gesendet) ist. Dieser Wert wird für den Benutzer festgelegt, wenn die Schaltfläche "Speichern"oder "Senden"gedrückt wird.</td>
      <td>Status_vod_c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Record Type</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Record Type</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>Anruf</td>
      <td>Suche nach dem -Aufruf. Jede Schlüsselmeldung ist mit einem -Aufruf verknüpft.</td>
      <td>Call2_vod_c</td>
      <td>Übergeordnet-Detail(call)</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>Kategorie</td>
      <td>Zeichnet die Nachrichtenkategorie der Nachricht auf. Wird hauptsächlich für die Berichterstellung verwendet.</td>
      <td>Category_vod_c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>CLM-Präsentationsname</td>
      <td>Stempelname der CLM-Präsentation</td>
      <td>clm_Presentation_Name_vod_c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>Schlüsselnachrichtenname</td>
      <td>Name der mit Stempel versehenen Schlüsselmeldung</td>
      <td>key_message_name_vod_c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>Produktbezeichnung</td>
      <td> </td>
      <td>Product_Name_c</td>
      <td>Formel (Text)</td>
    </tr>
    <tr>
      <td>Schlüsselmeldung aufrufen</td>
      <td>Reaktion</a>
      </td>
      <td>Liste der Reaktionen auf die Nachricht. Bearbeiten Sie die Auswahlliste, um die Reaktionswerte zu ändern.</td>
      <td>Reaction_vod_c</td>
      <td>Auswahlliste</td>
    </tr>
  </tbody>
</table>
