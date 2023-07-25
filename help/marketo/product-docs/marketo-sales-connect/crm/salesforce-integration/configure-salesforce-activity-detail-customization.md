---
description: Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 1%

---

# Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce und Marketo Sales Connect [muss verbunden sein](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* E-Mail-Aktivität über API protokollieren [muss aktiviert sein](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

Die Anpassung der Aktivitätsdetails ermöglicht es Administratoren, die Informationen zu konfigurieren, die beim Feld &quot;Salesforce-Aufgabe - Betreff&quot;protokolliert werden, wenn eine Aktivität/Erinnerungsaufgabe vom Typ &quot;Sales Connect&quot;mit Salesforce synchronisiert wird.

>[!NOTE]
>
>* Aktualisierungen am Betrefffeld in Sales Connect einer Erinnerungsaufgabe werden im Betrefffeld der entsprechenden Salesforce-Aufgabe angezeigt, wenn Sie die `{{activity_subject}}` dynamisches Feld in Ihrer Aktivitätsdetailanpassung.
>* Zeilenumbrüche werden bei der Protokollierung von Informationen in das Salesforce-Betrefffeld nicht unterstützt. Zeilenumbrüche im Editor zur Anpassung von Aktivitätsdetails werden entfernt, wenn ein Betreff einer Verkaufsaufgabe aktualisiert wird.

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
  <td>Aufrufaktivität</td>
 </tr>
</table>

Mit der Funktion können die folgenden Vorteile freigeschaltet werden:

* Durch die Anpassung der sichtbaren Informationen im Betrefffeld können Aktivitätsdetails in Salesforce problemlos für den Verkauf durchsucht werden.
* Administratoren können das Betrefffeld mit einer eindeutigen Kennung wie &quot;Mkto_sales&quot;taggen, damit Aktivitäten aus Sales Connect einfach identifiziert und von anderen E-Mail-Aktivitäten, Aufrufaktivitäten und Aufgaben unterschieden werden können.
* Reduzieren Sie den Bedarf an benutzerdefinierten Aktivitätsfeldern. Salesforce erzwingt Einschränkungen bei der Anzahl der benutzerdefinierten Aktivitätsfelder, wodurch eingeschränkt werden kann, welche Daten in Berichten verwendet werden können. Durch die Verwendung dynamischer Aktivitätsfelder zum Hinzufügen von Schlüsseldaten zur Betreffzeile können Sie die Anzahl der benutzerdefinierten Aktivitätsfelder reduzieren, die Sie in Ihrer Salesforce-Instanz erstellen müssen.
* Das Themenfeld der Aktivitäten und Aufgaben folgt einem einheitlichen Muster, das vom Sales Connect-Administrator definiert wird.

>[!NOTE]
>
>Wenn Sie E-Mail-Antworten als Aktivitäten an Salesforce protokollieren, werden sie nicht die Einstellungen für die Anpassung der Salesforce-Aktivitätsdetails verwenden. Stattdessen protokollieren sie als &quot;Antwort: E-Mail-Betreff.&quot;

## Unterstützte dynamische Aktivitätsfelder {#activity-dynamic-fields-supported}

Dynamische Felder der Aktivität Referenzinformationen zu Ihren Verkaufsaktivitäten zum Ausfüllen von Daten. Heute können sie mit der Anpassung von Salesforce-Aktivitätsdetails verwendet werden.

>[!NOTE]
>
>Wenn das dynamische Feld für eine bestimmte Aktivität/Aufgabe nicht mit Werten gefüllt werden soll, werden bei der Aktualisierung des Felds Salesforce Task - Subject keine Daten für dieses dynamische Feld ausgefüllt.

<table>
 <tr>
  <th>Feld</th>
  <th>Beschreibung</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Fügt den Aufgabentyp als E-Mail, Aufruf, InMail oder Benutzerdefiniert ein.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Füllt den Betreff der Aufgabe.</p>
      <p>Im Fall einer E-Mail wird die Betreffzeile der E-Mail ausgefüllt.</p>
      <p>Im Falle eines Aufrufs, inMail oder custom wird ein Wert aufgefüllt, wenn eine Erinnerungsaufgabe mit einem Wert im Feld "Aufgabenname/Betreff"erstellt wurde.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Wenn die Aktivität über eine Verkaufskampagne gestartet wurde, wird der Name der Verkaufskampagne ausgefüllt.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Wenn die Aktivität über eine Verkaufskampagne gestartet wurde, wird die Anzahl der Tage der Verkaufskampagne ausgefüllt, an denen diese Aktivität stattgefunden hat.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Wenn die Aktivität von einer Verkaufskampagne aus initiiert wurde, wird die Schrittnummer innerhalb der Verkaufskampagne aufgefüllt, an der diese Aktivität stattgefunden hat.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Wenn es sich bei der Aktivität um einen Aufruf handelt und ein Aufrufergebnis ausgewählt ist, wird der Ergebniswert des Aufrufs ausgefüllt.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Wenn es sich bei der Aktivität um einen Aufruf handelt und ein Anrufgrund ausgewählt ist, wird der Wert des Anrufergrunds ausgefüllt.</td>
 </tr>
</table>

## Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich.**

Überlegen Sie bei der Konfiguration Ihrer Aktivitätsdetails, welche Daten bei der Überprüfung des Aufgabenverlaufs in Salesforce am relevantesten für den Vertrieb sind.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Klicken **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Klicken **Einstellungen synchronisieren**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Fügen Sie im Editor für die Anpassung der Aktivitätsdetails den gewünschten freien Text hinzu. Text, den Sie hinzufügen, ist nicht dynamisch und bleibt für das Betrefffeld aller mit Salesforce synchronisierten Aufgaben unverändert.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Obwohl dies nicht erforderlich ist, kann es für einige Personen einfacher sein, zwischen den Daten zu unterscheiden, wenn sie in ein Subjektfeld in Salesforce eingefügt werden. Beispiel: `[Sales Connect] - {{Activity_type}}`

1. Fügen Sie die gewünschten dynamischen Felder hinzu, indem Sie auf die Schaltfläche **Dynamisches Feld hinzufügen** Schaltfläche.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Wählen Sie die gewünschten dynamischen Felder aus.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Klicken **Speichern**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce erzwingt eine Beschränkung von 255 Zeichen. Wenn Ihre Aktivitätsdetails diese Zahl überschreiten, werden sie abgeschnitten, um sicherzustellen, dass die Informationen im Betrefffeld Salesforce gespeichert werden.

>[!MORELIKETHIS]
>
>* [Synchronisierungseinstellungen](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Erinnern von Aufgabensynchronisierung mit Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Anpassung von Sales Connect für CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
