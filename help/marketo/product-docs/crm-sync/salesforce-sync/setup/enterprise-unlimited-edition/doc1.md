---
description: 'Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Unternehmen/Unbegrenzt) - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 1 von 3: Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)'
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Schritt 1 von 3: Hinzufügen der Marketo-Felder zu Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Sie müssen Zugriff auf Salesforce-APIs haben, um zwischen Marketo Engage und Salesforce synchronisieren zu können.

Marketo verwendet einen Satz von Feldern, um bestimmte Arten von Marketing-bezogenen Informationen zu erfassen. Wenn Sie diese Daten in Salesforce benötigen, befolgen Sie bitte die folgenden Anweisungen.

1. Erstellen Sie drei benutzerdefinierte Felder in Salesforce für die Lead- und Kontaktobjekte: Bewertung, Akquiseprogramm und Akquisedatum.
1. Ordnen Sie diese benutzerdefinierten Felder den Leads und Kontakten zu, sodass die Werte bei der Konvertierung in Salesforce übernommen werden.
1. Sie können bei Bedarf weitere Felder erstellen (siehe Tabelle unten).

Alle diese benutzerdefinierten Felder sind optional und müssen nicht zur Synchronisierung von Marketo und Salesforce verwendet werden. Als Best Practice empfehlen wir, Felder für Score, Akquise-Programm und Akquise-Datum zu erstellen.

## Hinzufügen von Marketo-Feldern zu Salesforce {#add-marketo-fields-to-salesforce}

Fügen Sie drei benutzerdefinierte Felder zu den Lead- und Kontaktobjekten in Salesforce hinzu, die oben aufgeführt sind. Weitere Informationen finden Sie in der Tabelle mit den verfügbaren Feldern am Ende dieses Abschnitts.

Führen Sie die folgenden Schritte für jedes der drei benutzerdefinierten Felder aus, um sie hinzuzufügen. Beginnen Sie mit der Bewertung.

1. Melden Sie sich bei Salesforce an und klicken Sie auf Setup.

   SCREENSHOT

1. Suchen Sie in der Schnellsuche nach dem Wort „Objekt“

   SCREENSHOT

1. Klicken Sie auf Objekt-Manager und suchen Sie nach „Leads“

   SCREENSHOT

1. Klicken Sie unter BESCHRIFTUNG auf Lead, und klicken Sie dann links auf Felder und Beziehungen .

   SCREENSHOT

1. Klicken Sie auf die Schaltfläche Neu auf der Seite „Felder und Beziehungen“

   SCREENSHOT

1. Wählen Sie den entsprechenden Feldtyp aus (für Score - Zahl; Akquise Programm - Text; Akquise - Datum/Uhrzeit).

   SCREENSHOT

1. Klicken Sie auf Weiter.

   SCREENSHOT

1. Geben Sie Feldbezeichnung, Länge und Feldname für das Feld ein, wie in der folgenden Tabelle dargestellt.

   TABELLE

   >[!NOTE]
   >
   >Salesforce hängt __c an Feldnamen an, wenn es sie zum Erstellen von API-Namen verwendet.

   SCREENSHOT

   >[!NOTE]
   >
   >Text- und Zahlenfelder erfordern eine Länge, Datums-/Uhrzeitfelder jedoch nicht. Eine Beschreibung ist optional.

1. Klicken Sie auf Weiter.

   SCREENSHOT

1. Legen Sie die Zugriffseinstellungen fest und klicken Sie auf Weiter:

   Alle Rollen auf „Sichtbar“ und „Schreibgeschützt“ einstellen

   Deaktivieren Sie das Kontrollkästchen Schreibgeschützt für das Profil des Synchronisierungsbenutzers:

   Wenn Sie einen Benutzer mit dem Profil eines Systemadministrators als Synchronisierungsbenutzer haben, deaktivieren Sie das Kontrollkästchen Schreibgeschützt für das Systemadministratorprofil (wie unten dargestellt)
Wenn Sie ein benutzerdefiniertes Profil für den Synchronisierungsbenutzer erstellt haben, deaktivieren Sie das Kontrollkästchen Schreibgeschützt für dieses benutzerdefinierte Profil

   SCREENSHOT

1. Wählen Sie die Seiten-Layouts aus, in denen das Feld angezeigt werden soll.

   SCREENSHOT

1. Klicken Sie auf Speichern und neu , um zurückzugehen und jedes der beiden anderen benutzerdefinierten Felder zu erstellen. Klicken Sie auf Speichern , wenn Sie alle drei Aufgaben abgeschlossen haben.

   SCREENSHOT

* Suchen Sie im Objekt-Manager nach „Kontakte“. Klicken Sie auf Felder und Beziehungen.
* Führen Sie die Schritte 5 bis 12 für die Felder Score, Akquisitionsdatum und Akquise-Programm im Kontaktobjekt aus, genau wie Sie es für das Lead-Objekt getan haben.
* Optional können Sie das obige Verfahren für alle zusätzlichen benutzerdefinierten Felder aus dieser Tabelle verwenden.

  TABELLE

  >[!NOTE]
  >
  >Werte in den von Marketo automatisch zugewiesenen Feldern sind nach der Erstellung des neuen Felds nicht sofort in Salesforce verfügbar. Marketo synchronisiert die Daten mit Salesforce bei der nächsten Aktualisierung des Datensatzes auf einem der Systeme (d. h. bei einer Aktualisierung eines der Felder, die zwischen Marketo und Salesforce synchronisiert werden).

## Zuordnen benutzerdefinierter Felder für Konversionen {#map-custom-fields-for-conversions}

Ein benutzerdefiniertes Feld auf dem Lead-Objekt in Salesforce sollte einem Kontaktfeld auf dem Kontaktobjekt zugeordnet werden, damit die Daten übertragen werden, wenn eine Konversion stattfindet.

1. Klicken Sie oben rechts auf Setup.

   SCREENSHOT

1. Suchen Sie in der Schnellsuche nach dem Wort „Objekt“

   SCREENSHOT

1. Gehen Sie zum Abschnitt Benutzerdefinierte Lead-Felder und Beziehungen und klicken Sie auf Lead-Felder zuordnen .

   SCREENSHOT

1. Klicken Sie auf das Dropdown-Menü neben dem Feld, das Sie zuordnen möchten, und zwar auf der entsprechenden Registerkarte Konto, Kontakt oder Opportunity .

   SCREENSHOT

1. Wählen Sie das entsprechende benutzerdefinierte Feld Kontakt aus.

   SCREENSHOT

1. Wiederholen Sie die obigen Schritte für alle anderen Felder, die Sie erstellt haben.

1. Klicken Sie abschließend auf Speichern .
