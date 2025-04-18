---
description: Konfigurieren der Anpassung von Salesforce-Aktivitätsdetails - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren der Anpassung von Salesforce-Aktivitätsdetails
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 1%

---

# Konfigurieren der Anpassung von Salesforce-Aktivitätsdetails {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce- und Sales Insight-Aktionen [müssen verbunden sein](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* E-Mail-Aktivität über API protokollieren [muss aktiviert sein](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

Mit der Anpassung von Aktivitätsdetails können Administratoren die Informationen konfigurieren, die beim Synchronisieren einer Aktivität/Erinnerungsaufgabe für Sales Insight-Aktionen mit Salesforce in das Feld &quot;Salesforce-Aufgabe - Betreff“ protokolliert werden.

>[!NOTE]
>
>* Aktualisierungen des Betrefffelds in Sales Insights-Aktionen einer Erinnerungsaufgabe werden im Betrefffeld der entsprechenden Salesforce-Aufgabe angezeigt, wenn Sie das dynamische Feld &quot;`{{activity_subject}}`&quot; in Ihrer Anpassung der Aktivitätsdetails verwenden.
>* Zeilenumbrüche werden beim Protokollieren von Informationen im Salesforce-Betrefffeld nicht unterstützt. Alle Zeilenumbrüche im Editor zur Anpassung von Aktivitätsdetails werden entfernt, wenn ein Betreff für eine Verkaufsaufgabe aktualisiert wird.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>InMail-Erinnerungsaufgabe</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>E-Mail-Aktivität</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Aktivität „Aufruf“</td>
 </tr>
</table>

Mit der Funktion können die folgenden Vorteile erzielt werden:

* Durch die Anpassung der Informationen, die im Betrefffeld angezeigt werden, können Aktivitätsdetails in Salesforce einfach für den Vertrieb durchsucht werden.
* Admins können das Betrefffeld mit einer eindeutigen Kennung wie „moto_sales“ versehen, damit Aktivitäten aus Sales-Insight-Aktionen einfach identifiziert und von anderen E-Mail-Aktivitäten, Anrufaktivitäten und Aufgaben unterschieden werden können.
* Reduzieren Sie den Bedarf an benutzerdefinierten Aktivitätsfeldern. Salesforce erzwingt Beschränkungen für die Anzahl der benutzerdefinierten Aktivitätsfelder, wodurch eingeschränkt werden kann, welche Daten in Berichten verwendet werden können. Wenn Sie dynamische Aktivitätsfelder verwenden, um Schlüsseldaten zur Betreffzeile hinzuzufügen, können Sie die Anzahl der benutzerdefinierten Aktivitätsfelder reduzieren, die Sie in Ihrer Salesforce-Instanz erstellen müssen.
* Das Betrefffeld der Aktivitäten und Aufgaben folgt einem konsistenten Muster, das vom Sales Insight Actions Admin definiert wird.

>[!NOTE]
>
>Wenn Sie E-Mail-Antworten als Aktivitäten in Salesforce protokollieren, werden die Einstellungen zur Anpassung der Salesforce-Aktivitätsdetails nicht verwendet. Stattdessen wird „Antwort: E-Mail-Betreff“ protokolliert.

## Unterstützte dynamische Aktivitätsfelder {#activity-dynamic-fields-supported}

Dynamische Aktivitätsfelder : Referenzinformationen zu Ihren Vertriebsaktivitäten, um Daten zu füllen. Heute können sie mit der Anpassung von Salesforce-Aktivitätsdetails verwendet werden.

>[!NOTE]
>
>Wenn kein Wert zum Ausfüllen des dynamischen Felds für eine bestimmte Aktivität/Aufgabe vorhanden ist, werden beim Aktualisieren des Felds Salesforce-Aufgabe - Betreff keine Daten für dieses dynamische Feld ausgefüllt.

<table>
 <tr>
  <th>Feld</th>
  <th>Beschreibung</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>füllt den Aufgabentyp als E-Mail, Anruf, InMail oder Benutzerdefiniert aus.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Befüllt den Betreff der Aufgabe.</p>
      <p>Bei E-Mails wird die Betreffzeile der E-Mail ausgefüllt.</p>
      <p>Bei einem -Aufruf, inMail oder einem benutzerdefinierten Aufruf wird ein Wert eingetragen, wenn im Feld Aufgabenname/Betreff eine Erinnerungsaufgabe mit einem Wert erstellt wurde.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Wenn die Aktivität von einer Verkaufskampagne initiiert wurde, wird der Name der Verkaufskampagne angegeben.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Wenn die Aktivität von einer Verkaufskampagne initiiert wurde, wird die Tagesnummer der Verkaufskampagne angegeben, an der diese Aktivität stattgefunden hat.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Wenn die Aktivität von einer Verkaufskampagne initiiert wurde, wird die Schrittnummer innerhalb der Verkaufskampagne am Tag ausgefüllt, an dem diese Aktivität stattgefunden hat.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Wenn es sich bei der Aktivität um einen Aufruf handelt und ein Aufrufergebnis ausgewählt wird, wird der Wert für das Aufrufergebnis ausgefüllt.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Wenn es sich bei der Aktivität um einen Aufruf handelt und ein Anrufgrund ausgewählt ist, wird der Wert für den Anrufgrund ausgefüllt.</td>
 </tr>
</table>

## Konfigurieren der Anpassung von Salesforce-Aktivitätsdetails {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich.**

Berücksichtigen Sie bei der Konfiguration Ihrer Aktivitätsdetails, welche Daten für den Vertrieb am relevantesten sind, wenn Sie den Aufgabenverlauf in Salesforce überprüfen.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Auf **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Klicken Sie auf **Einstellungen synchronisieren**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Fügen Sie im Editor zur Anpassung der Aktivitätsdetails einen beliebigen freien Text hinzu. Hinzugefügter Text ist nicht dynamisch und bleibt für das Betrefffeld aller mit Salesforce synchronisierten Aufgaben unverändert.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Wenn hinzugefügter Text in gerade Klammern eingeschlossen wird, ist dies zwar nicht erforderlich, doch kann es für manche Personen einfacher sein, zwischen den Daten zu unterscheiden, wenn sie in ein Betrefffeld in Salesforce eingefügt werden. Beispiel: `[Sales Insight Actions] - {{Activity_type}}`

1. Fügen Sie alle gewünschten zusätzlichen dynamischen Felder hinzu, indem Sie auf die Schaltfläche **Dynamisches Feld hinzufügen** klicken.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Wählen Sie die gewünschten dynamischen Felder aus.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce setzt eine Beschränkung auf 255 Zeichen durch. Wenn Ihre Aktivitätsdetails diesen Wert überschreiten, werden sie abgeschnitten, um sicherzustellen, dass die Informationen im Salesforce-Betrefffeld gespeichert werden.

>[!MORELIKETHIS]
>
>* [Verkaufsaktivitäten mit Salesforce synchronisieren](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Erinnerungsaufgabe - Synchronisieren mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
