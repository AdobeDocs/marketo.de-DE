---
description: Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails
hide: true
hidefromtoc: true
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# Konfigurieren der Anpassung der Salesforce-Aktivitätsdetails {#configure-salesforce-activity-detail-customization}

Die Anpassung der Aktivitätsdetails ermöglicht es Administratoren, die Informationen zu konfigurieren, die beim Feld &quot;Salesforce-Aufgabe - Betreff&quot;protokolliert werden, wenn eine Aktivität/Erinnerungsaufgabe vom Typ &quot;Sales Connect&quot;mit Salesforce synchronisiert wird.

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
  <td>{{activity_type}</td>
  <td>Fügt den Aufgabentyp als E-Mail, Aufruf, InMail oder Benutzerdefiniert ein.</td>
 </tr>
 <tr>
  <td>{{activity_subject}</td>
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
  <td>{{call_result}</td>
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

PICC

1. Klicken **Salesforce**.

PICC

1. Klicken **Einstellungen synchronisieren**.

PICC

1. Fügen Sie im Editor zur Anpassung der Aktivitätsdetails den gewünschten freien Text hinzu. Dieser bleibt für das Betrefffeld aller mit Salesforce synchronisierten Aufgaben unverändert.

1. Fügen Sie die hinzuzufügenden dynamischen Felder hinzu, indem Sie auf die Schaltfläche Dynamisches Feld klicken und die zu verwendenden dynamischen Felder aus der Liste auswählen.

1. Klicken **Speichern**.

>[!NOTE]
>
>Salesforce erzwingt eine Beschränkung von 255 Zeichen. Wenn Ihre Aktivitätsdetails diese Anzahl überschreiten, werden sie abgeschnitten, um sicherzustellen, dass die Informationen im Betrefffeld Salesforce gespeichert werden können.

>[!MORELIKETHIS]
>
>* [Synchronisierungseinstellungen](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Erinnern von Aufgabensynchronisierung mit Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Anpassung von Sales Connect für CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)

