---
description: Deinstallieren von Marketo Sales Connect von Salesforce Classic - Marketo Docs - Produktdokumentation
title: Deinstallieren von Marketo Sales Connect von Salesforce Classic
exl-id: 17078054-a615-4f2f-bfde-f28fd3ff6f48
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 8%

---

# Deinstallieren von Marketo Sales Connect von Salesforce Classic {#uninstall-marketo-sales-connect-from-salesforce-classic}

Hier erfahren Sie, wie Sie das Marketo Sales Connect-Package aus Ihrem Salesforce-Konto deinstallieren, sobald Sie mit der Verwendung von Sales Insight-Aktionen beginnen.

## Felder für Verkaufsverbindung aus Seitenlayout entfernen {#remove-sales-connect-fields-from-page-layout}

1. Klicken Sie in Salesforce Classic auf **Setup**.

   ![](assets/uninstall-salesforce-classic-customization-package-1.png)

1. Erweitern Sie in der linken Navigationsleiste unter &quot;Erstellen&quot;die Option Anpassen (aber nicht klicken) und dann Leads. Wählen Sie dann **Seitenlayouts** aus.

   ![](assets/uninstall-salesforce-classic-customization-package-2.png)

1. Klicken Sie neben Lead-Layout auf **Bearbeiten** .

   ![](assets/uninstall-salesforce-classic-customization-package-3.png)

1. Wählen Sie in der Konsole **Felder** aus. Suchen Sie in der Schnellsuche nach &quot;MSC&quot;. Alle ausgegrauten Felder wurden Ihrem Seitenlayout hinzugefügt. Sie werden sie löschen müssen.

   ![](assets/uninstall-salesforce-classic-customization-package-4.png)

   >[!NOTE]
   >
   >Wenn keines der Felder ausgegraut ist, bedeutet dies, dass Sie sie nicht zum Seitenlayout hinzugefügt haben. Sie können diesen Abschnitt überspringen.

1. Scrollen Sie zu dem Abschnitt, in dem Ihre benutzerdefinierten Felder für Sales Connect vorhanden sind.

   ![](assets/uninstall-salesforce-classic-customization-package-5.png)

1. Es gibt 10 Typen von MSC-Feldern, die zu diesem Abschnitt hinzugefügt werden können. Entfernen Sie alle hinzugefügten Felder oder löschen Sie einfach den gesamten Abschnitt.

1. Klicken Sie abschließend auf **Quick Save** .

   ![](assets/uninstall-salesforce-classic-customization-package-6.png)

## Entfernen von Verkaufsverbindungs-Schaltflächen aus Seitenlayouts {#remove-sales-connect-buttons-from-page-layouts}

1. Wählen Sie in der Konsole (Schritt 4 oben) **Schaltflächen** aus. Suchen Sie &quot;MSC&quot;. Alle ausgegrauten Schaltflächen wurden Ihrem benutzerdefinierten Schaltflächenabschnitt hinzugefügt. Sie werden sie löschen müssen.

   ![](assets/uninstall-salesforce-classic-customization-package-7.png)

   >[!NOTE]
   >
   >Wenn keine der Schaltflächen ausgegraut ist, bedeutet dies, dass Sie sie nicht hinzugefügt haben. Sie können diesen Abschnitt überspringen.

1. Ziehen Sie die MSC-Schaltflächen aus dem Abschnitt Benutzerdefinierte Schaltflächen in die Konsole.

   ![](assets/uninstall-salesforce-classic-customization-package-8.png)

1. Klicken Sie abschließend auf **Quick Save** .

   ![](assets/uninstall-salesforce-classic-customization-package-9.png)

## Entfernen von Verkaufsverbindungs-Feldern aus dem Abschnitt &quot;Aktivitätsverlauf&quot; {#remove-sales-connect-fields-from-activity-history-section}

1. Scrollen Sie zum unteren Rand der Seite zum Listenbereich Aktivitätsverlauf und klicken Sie auf das Schraubenschlüsselsymbol.

   ![](assets/uninstall-salesforce-classic-customization-package-10.png)

1. Wählen Sie im Bereich Ausgewählte Felder die Felder Verkaufsverbindung aus und klicken Sie auf den Pfeil Entfernen . Klicken Sie abschließend auf **OK** .

   ![](assets/uninstall-salesforce-classic-customization-package-11.png)

   >[!NOTE]
   >
   >Die Abkürzung MSE _ist_ Sales Connect. Es ist nur der vorherige Name &quot;Marketo Sales Engage&quot;.

1. Klicken Sie auf **Speichern** , wenn Sie mit der Lead-Seite fertig sind.

## Entfernen Sie die Aktionsschaltflächen &quot;Sales Connect&quot;-Massenaktion aus der Lead-Listenansicht. {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. Erweitern Sie in der linken Navigationsleiste unter &quot;Erstellen&quot;die Option Anpassen (aber nicht klicken) und dann Leads. Wählen Sie dann **Layouts durchsuchen** aus.

   ![](assets/uninstall-salesforce-classic-customization-package-12.png)

1. Klicken Sie neben der Leads-Listenansicht auf **Bearbeiten**.

   ![](assets/uninstall-salesforce-classic-customization-package-13.png)

1. Wählen Sie **Zu MSC-Kampagne hinzufügen (klassisch)**, **E-Mail mit MSC (klassisch)** und **Zum MSC pushen (klassisch)** und klicken Sie auf den Pfeil &quot;Entfernen&quot;. Klicken Sie dann auf **Speichern**.

   ![](assets/uninstall-salesforce-classic-customization-package-14.png)

Die Schaltflächen in der Liste der Leads sollten nicht mehr angezeigt werden.

## MSC-Konfiguration für Kontakte entfernen {#remove-msc-configuration-for-contacts}

1. Klicken Sie in Salesforce auf **Einrichtung**.

1. Erweitern Sie in der linken Navigationsleiste unter &quot;Erstellen&quot;die Option Anpassen (aber nicht klicken) und dann Kontakte. Wählen Sie dann **Seitenlayouts** aus.

1. Klicken Sie neben Kontaktlayout auf **Bearbeiten**.

1. Wiederholen Sie die Schritte für alle drei Abschnitte.

## MSC-Konfiguration für Opportunity entfernen {#remove-msc-configuration-for-opportunity}

1. Klicken Sie in Salesforce auf **Einrichtung**.

1. Erweitern Sie in der linken Navigationsleiste unter &quot;Erstellen&quot;die Option Anpassen (aber nicht klicken) und anschließend die Option Chancen . Wählen Sie dann **Seitenlayouts** aus.

1. Klicken Sie neben &quot;Opportunity Layout&quot;auf **Edit**.

1. Wiederholen Sie die Schritte für alle drei Abschnitte.

Die Opportunity-Ansicht hat nur eine Schaltfläche - &quot;MSE-E-Mail senden&quot;- und die folgenden Felder:

![](assets/uninstall-salesforce-classic-customization-package-15.png)

## MSC-Konfiguration für Konto entfernen {#remove-msc-configuration-for-account}

1. Klicken Sie in Salesforce auf **Einrichtung**.

1. Erweitern Sie in der linken Navigationsleiste unter &quot;Erstellen&quot;die Option Anpassen (aber nicht klicken) und klicken Sie dann auf &quot;Konto&quot;. Wählen Sie dann **Seitenlayouts** aus.

1. Klicken Sie neben Kontolayout auf **Bearbeiten**.

1. Wiederholen Sie die Schritte für alle drei Abschnitte.

Die Kontoansicht hat nur eine Schaltfläche - &quot;MSE-E-Mail senden&quot;- und die folgenden Felder:

![](assets/uninstall-salesforce-classic-customization-package-16.png)

## Marketo Sales Outbox entfernen {#remove-marketo-sales-outbox}

1. Klicken Sie in Salesforce oben auf Ihrem Bildschirm auf die Registerkarte **+** .

1. Klicken Sie auf **Meine Registerkarten anpassen**.

1. Wählen Sie rechts die Option Marketo Sales Outbox aus. Klicken Sie auf den Pfeil Entfernen und dann auf **Speichern**.

## Sales Connect-Paket löschen {#delete-sales-connect-package}

Nachdem Sie alle Objekte aus Ihrem Salesforce-Konto entfernt haben, führen Sie die folgenden Schritte aus.

1. Klicken Sie in Salesforce auf **Einrichtung**.

1. Geben Sie in das Feld &quot;Schnellsuche&quot;die Option &quot;Apex-Klassen&quot;ein.

1. Klicken Sie auf **Löschen** neben allen Einträgen &quot;MarketoSalesConnectionCustomization&quot;oder &quot;MarketoSalesEngageCustomization&quot;in Ihrer Liste.

Das war’s schon!

Im Folgenden finden Sie eine Liste aller Objekte, die aus Ihrer Salesforce-Instanz entfernt werden müssen:

## Anpassungsdetails für Sales Connect {#sales-connect-customization-details}

<table>
 <tr>
  <th>Benutzerdefinierte Aktivitätsfelder</th>
  <th>Beschreibung</th>
  <th>Typ</th>
  <th>Datentyp</th>
 </tr>
 <tr>
  <td>Lokale Präsenz-ID des MSC-Aufrufs</td>
  <td>Als Benutzer kann ich "Lokale Präsenz"als Option wählen, wenn ich über MSC Phone anrufe. Eingehende Anrufe zeigen eine lokale Nummer für den Empfänger an</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL zur Aufzeichnung von MSC-Aufrufen</td>
  <td>Aufrufe können aufgezeichnet werden und ein Link für die Aufzeichnung wird hier protokolliert </td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC Campaign</td>
  <td>Protokollname der MSC-Kampagne, auf der sich der Kontakt/Lead befindet</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-Kampagnen-URL</td>
  <td>Protokolliert die URL der Kampagne, die in MSC erstellt wurde. Durch Klicken auf diese Schaltfläche wird die Kampagne in der MSC-Web-App geöffnet.</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>Aktueller Schritt einer MSC-Kampagne</td>
  <td>Wenn sich ein Kontakt/Lead in einer Kampagne befindet, protokolliert dieses Feld den Namen des Schritts, in dem er sich gerade befindet</td>
  <td>Aktivität</td>
  <td>Kontrollkästchen</td>
 </tr>
 <tr>
  <td>Angezeigte MSC-E-Mail-Anlage</td>
  <td>Protokolliert Daten, wenn eine E-Mail mit einem Anhang gesendet wird, der vom Empfänger angezeigt wird</td>
  <td>Aktivität</td>
  <td>Kontrollkästchen</td>
 </tr>
 <tr>
  <td>MSC-E-Mail angeklickt</td>
  <td>Protokolliert ein Häkchen, wenn der Empfänger auf einen Link in der E-Mail klickt</td>
  <td>Aktivität</td>
  <td>Kontrollkästchen</td>
 </tr>
 <tr>
  <td>MSC-E-Mail beantwortet</td>
  <td>Protokolliert ein Häkchen, wenn der Empfänger auf die E-Mail antwortet</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-E-Mail-Status</td>
  <td>Zeigt an, ob eine E-Mail gesendet/in Bearbeitung/abgestürzt wurde (das Tracking nicht zugestellter E-Mails hängt vom verwendeten Versandkanal ab)</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-E-Mail-Vorlage</td>
  <td>Logname der MSC-Vorlage, die in der an den Lead/Kontakt gesendeten E-Mail verwendet wurde</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL der MSC-E-Mail-Vorlage</td>
  <td>Protokolliert die URL auf die Vorlage, die in MSC erstellt wurde. Durch Klicken auf diese Option wird die Vorlage in der MSC-Web-App geöffnet.</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-E-Mail-URL</td>
  <td>Durch Klicken auf diese URL wird das Befehlszentrum in MSC geöffnet und die Registerkarte "People Detail View history"abgerufen, auf der der Benutzer die gesendete E-Mail sehen kann</td>
  <td>Aktivität</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>Angezeigte MSC-E-Mail</td>
  <td>Protokolliert ein Häkchen, wenn der Empfänger eine E-Mail anzeigt</td>
  <td>Aktivität</td>
  <td>Kontrollkästchen</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC-Protokollierungsfeld für Datenaggregation</th>
  <th>Beschreibung</th>
  <th>Typ</th>
  <th>Datentyp</th>
 </tr>
 <tr>
  <td>MSC - Letzte Marketinginteraktion</td>
  <td>Letzte eingehende Interaktion aus Marketing</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Daten und Zeit</td>
 </tr>
 <tr>
  <td>MSC - Datum der letzten Marketing-Interaktion</td>
  <td>Zeitstempel der Interaktion vom Marketing</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Daten und Zeit</td>
 </tr>
 <tr>
  <td>MSC - Letzte Marketing-Interaktion Desc</td>
  <td>Beschreibung der Interaktion</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Letzte Marketinginteraktion - Source</td>
  <td>Source der Marketinginteraktion</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Letzter Marketing-Interaktionstyp</td>
  <td>Art der Interaktion (z. B. Web-Aktivität)</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Letzte Aktivität nach Vertrieb</td>
  <td>Letzte ausgehende Aktivität des Verkaufsteams</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Daten und Zeit</td>
 </tr>
 <tr>
  <td>MSC - Zuletzt geantwortet</td>
  <td>Letzte E-Mail-Antwort auf die E-Mail "Verkauf"</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Daten und Zeit</td>
 </tr>
 <tr>
  <td>MSC - Aktuelle Vertriebskampagne</td>
  <td>Protokollname der MSC-Kampagne, auf der sich der Kontakt/Lead befindet</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Letzte Interaktion bei Verkäufen</td>
  <td>Letzte eingehende Interaktion aus Verkäufen</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Daten und Zeit</td>
 </tr>
 <tr>
  <td>MSC - Opt-out</td>
  <td>Abmeldefeld</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
  <td>Kontrollkästchen</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC-Schaltflächen</th>
  <th>Beschreibung</th>
  <th>Typ</th>
 </tr>
 <tr>
  <td>MSC-E-Mail senden</td>
  <td>Senden von Verkaufs-E-Mails von Salesforce</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Opportunity</td>
 </tr>
 <tr>
  <td>Zu MSC Campaign hinzufügen</td>
  <td>Zu MSC-Kampagnen von Salesforce hinzufügen</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Push to MSC</td>
  <td>Push-Kontakt von Salesforce zu MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Aufruf mit MSC</td>
  <td>Verkaufsaufrufe von Salesforce durchführen</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC Bulk Action Buttons</th>
  <th>Beschreibung</th>
  <th>Typ</th>
 </tr>
 <tr>
  <td>Zu MSC Campaign hinzufügen (Classic)</td>
  <td>Zu MSC-Kampagnen von Salesforce hinzufügen</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Push to MSC (Classic)</td>
  <td>Push-Kontakt von Salesforce zu MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>E-Mail mit MSC (Classic)</td>
  <td>E-Mail mit MSC von Salesforce</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
</table>
