---
description: Synchronisieren von Meldungen zu Aufrufen und Anrufen - Marketo-Dokumente - Produktdokumentation
title: Nachrichten zu Aufruf- und Aufrufschlüsseln synchronisieren
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 10%

---

# Nachrichten zu Aufruf- und Aufrufschlüsseln synchronisieren {#syncing-call-and-call-key-messages}

Die Nachrichtenobjekte „Call and Call Key“ in Veeva CRM werden standardmäßig mit Marketo Engage synchronisiert. Marketo synchronisiert Daten, die bis zu sechs Monate alt sind, basierend auf dem Erstellungsdatum des Anrufs.

>[!NOTE]
>
>Marketo speichert Anrufdaten bis zu sechs Monate ab dem Anrufdatum.

**Welche Trigger/Filter beziehen sich auf die Meldung „Aufruf- und Aufrufschlüssel“**

Auslöser:

* Zu Aufruf hinzugefügt
* Aus Aufruf entfernt
* Zu Anrufschlüsselnachricht hinzugefügt
* Aus Anrufschlüsselmeldung entfernt
* Aktualisierter Aufruf
* Aktualisierte Meldung zum Aufrufschlüssel

Filter:

* Hat Aufruf
* Hat Anrufschlüsselmeldung

Die folgenden Felder in den Meldungen zum Aufruf und Aufrufschlüssel werden synchronisiert und können als Einschränkungen und Trigger verwendet werden.

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
      <td>Suchen Sie nach dem Konto, mit dem der Aufruf verknüpft ist.</td>
      <td>Account_vod__c</td>
      <td>Lookup (Konto)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Aufruftyp</td>
      <td>Aufruftyp, der vom System basierend auf Typ und Inhalt des Aufrufs beibehalten wird. Dieses Feld wird zu Berichtszwecken verwendet. Gültige Werte sind: Nur Detail, Detail mit Beispiel, Gruppendetails, Gruppendetail mit Beispiel, Nur Beispiel. Diese Werte sollten nicht geändert werden, aber die Übersetzungen für diese Auswahllisten können geändert werden. Teilnehmer haben denselben Aufruftyp wie der Header-Aufruf. Bei einem Gruppenaufruf mit 3 Fachleuten haben alle 4 Datensätze den Aufruftyp „Gruppendetails“</td>
      <td>call_type_vod__c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
     <td>Anruf</td>
      <td>Kontakt</td>
      <td>Suchen Sie nach dem Kontakt (falls vorhanden), mit dem der Aufruf verknüpft ist.</td>
      <td>Kontakt_vod__c</td>
      <td>Lookup(contact)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Datum</td>
      <td>Das Datum des Anrufs, an dem er zum ersten Mal gespeichert oder gesendet wurde. Dieses Feld wird über einen Trigger auf das aktuelle Datum festgelegt, wenn weder das Datums- noch das Datums-/Uhrzeitfeld angegeben ist.</td>
      <td>call_date_vod__c</td>
      <td>Datum</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Ist übergeordneter Anruf?</td>
      <td>Formelfeld, um zu bestimmen, ob der Anrufdatensatz der übergeordnete Anrufdatensatz oder ein Teilnehmeranrufdatensatz ist. 1 gibt an, dass der Datensatz der übergeordnete Aufruf ist. 0 zeigt an, dass es sich um einen Teilnehmeraufruf handelt.</td>
      <td>is_parent_call_vod__c</td>
      <td>Formel (Zahl)</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Status</td>
      <td>Status des Anrufs - Geplant, gespeichert oder gesendet. Verwenden Sie das Übersetzungs-Workbench, um die Anzeigewerte zu ändern. Die Trigger bei Aufruf sehen in diesem Feld, ob der Aufruf gesperrt (gesendet) ist. Dieser Wert wird für den Benutzer festgelegt, wenn die Schaltfläche Speichern oder Senden gedrückt wird.</td>
      <td>Status_vod__c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
      <td>Anruf</td>
      <td>Art des Eintrags</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Art des Eintrags</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>Anruf</td>
      <td>Nachschlagen des Anrufs. Jede Schlüsselbotschaft ist mit einem Aufruf verknüpft.</td>
      <td>call2_vod__c</td>
      <td>master-detail(call)</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>Kategorie</td>
      <td>Zeichnet die Kategorie der Nachricht auf. Wird hauptsächlich für das Reporting verwendet.</td>
      <td>category_vod__c</td>
      <td>Auswahlliste</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>CLM-Präsentationsname</td>
      <td>Gestempelter CLM-Präsentationsname</td>
      <td>clm_presentation_name_vod__c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>Name der Schlüsselmeldung</td>
      <td>Name der Schlüsselmeldung mit Stempel</td>
      <td>key_message_name_vod__c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>Produktname</td>
      <td> </td>
      <td>product_name__c</td>
      <td>Formel (Text)</td>
    </tr>
    <tr>
      <td>Schlüsselnachricht aufrufen</td>
      <td>Reaktion</a>
      </td>
      <td>Auswahlliste der Reaktionen auf die Nachricht. Bearbeiten Sie die Auswahlliste, um die Reaktionswerte zu ändern.</td>
      <td>Reaction_vod__c</td>
      <td>Auswahlliste</td>
    </tr>
  </tbody>
</table>
