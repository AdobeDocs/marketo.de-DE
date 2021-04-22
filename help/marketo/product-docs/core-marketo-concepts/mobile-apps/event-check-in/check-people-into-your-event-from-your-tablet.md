---
unique-page-id: 2949839
description: Überprüfen Sie Personen auf Ihrem Tablet - Marketo Docs - Produktdokumentation auf Ihr Ereignis.
title: Personen von Ihrem Tablet in Ihr Ereignis einchecken
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Personen auf Ihrem Tablet {#check-people-into-your-event-from-your-tablet} in Ihr Ereignis einchecken

Wenn Personen in Ihrem Ereignis angezeigt werden, finden Sie deren Informationen in der App. Nach dem Check-in werden sie beim Synchronisieren mit Marketo zum Status &quot;Angehalten&quot;befördert.

Die App funktioniert auf dem iPad und Android gleich, mit Ausnahme kleinerer Layout- und Designunterschiede.

>[!PREREQUISITES]
>
>* Erstellen Sie ein Ereignis in Marketo und füllen Sie es mit eingeladenen und registrierten Personen aus.
>* Laden Sie die Tablet-App für [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) oder [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8) herunter


## Registrierte Gäste {#check-in-registered-guests}

1. Tippen Sie auf das App-Symbol auf Ihrem iPad oder Android-Tablet.

1. Tippen Sie auf **Anmelden**, um die Marketo Ereignis-App zu starten.

   ![](assets/1.jpg)

1. Geben Sie Ihren Marketo-Benutzernamen und Ihr Kennwort ein und klicken Sie auf **Anmelden**.

   >[!NOTE]
   >
   >Sie müssen über eine Rolle mit Zugriff auf die Datenbank verfügen, um Benutzer in der App anzuzeigen.

1. Wählen Sie ein **Ereignis**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Es werden nur Ereignis-Programms (mit Ausnahme von Webinaren) angezeigt, die eine Woche vor und eine Woche nach dem heutigen Datum geplant sind.

1. Suchen Sie auf dem Startbildschirm nach registrierten Gästen. Um eine Person in der Liste zu finden, können Sie:

   * Scrollen, um einen Namen zu suchen
   * Geben Sie einen Namen in das Suchfeld ein
   * Springen Sie zu einem bestimmten Anfangsbuchstaben des Nachnamens, indem Sie auf der rechten Seite der Liste darauf tippen

   >[!NOTE]
   >
   >Der Vorgang ist auf dem iPad und Android gleich, aber die Bildschirme unterscheiden sich, und Elemente können sich an unterschiedlichen Positionen befinden. Dieser Artikel enthält die iPad-Oberfläche. Vergleichen Sie den Android-Bildschirm in diesem Abschnitt als Referenz.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Tippen Sie auf den ausgewählten Namen und dann im Personendatensatz auf **Check-in**.

   ![](assets/img-0068-35-hands.png)

Der Gast hat jetzt den Status &quot;Angenommen&quot;und erhält ein Häkchen. Der Personendatensatz wird bei der Synchronisierung mit Marketo aktualisiert. Der rote Zähler auf der Synchronisierungsschaltfläche wird inkrementiert, um die Anzahl der Check-ins seit der letzten Synchronisierung mit Marketo anzuzeigen. Die Schaltfläche &quot;Synchronisieren&quot;sieht anders aus und befindet sich für iPad und Android an einem anderen Speicherort:

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Wenn eine Person eingeladen wurde, sich aber nicht registriert hat, können Sie nach dem Namen suchen, indem Sie auf **Suche auf Server** klicken, direkt unterhalb des Suchfelds. Der Status &quot;Eingeladen&quot;ändert sich für das Ereignis in **Anwesend**.

## Neue Person auf dem Tablet {#create-a-new-person-on-the-tablet} erstellen

Sie können Gäste, die keine Personen sind, manuell in Ihre Marketo-Datenbank aufnehmen. Sie werden automatisch eingecheckt und Ihrer Datenbank hinzugefügt, wenn Sie mit Marketo synchronisieren.

1. Klicken Sie auf **Hinzufügen**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Füllen Sie so viele grundlegende Informationsfelder wie möglich aus und tippen Sie auf **Fertig**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Sie können nur die vorhandenen Felder verwenden. Sie können keine benutzerdefinierten erstellen.

   >[!CAUTION]
   >
   >Überprüfen Sie die E-Mail-Adresse bei der Dublette. Andere Felder können später korrigiert werden, aber die E-Mail-Adresse ist die primäre Methode, um den Gast zu kontaktieren.

Die neue Person ist als bei Ihrem Ereignis eingecheckt registriert und wird bei der Synchronisierung mit Marketo der Marketo-Datenbank mit dem Status &quot;Beendet&quot;hinzugefügt.

## Umkehren eines Check-ins {#reverse-a-check-in}

Wenn Sie versehentlich eine Person, _vor der Synchronisierung mit Marketo_, eingecheckt haben, können Sie den Status &quot;Teilnehmer&quot;umkehren.

1. Tippen Sie in der Liste auf den Namen und im Personensatz auf **Rückgängig**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Alles fest!

## Einen Personensatz beim Check-In bearbeiten {#edit-a-person-record-at-check-in}

Sie können Gastinformationen direkt am Ereignis hinzufügen und ändern!

1. Tippen Sie auf den Namen in der Liste &quot;people&quot;und dann auf **Edit**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Bearbeiten Sie die Felder und fügen Sie Informationen hinzu. Tippen Sie dann auf **Fertig**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >In Android kann die Schaltfläche **Fertig** ausgeblendet sein. Blättern Sie nach unten, um es zu finden.

Die Informationen werden aktualisiert, wenn Sie die App mit Marketo synchronisieren.

## Synchronisieren der App mit Marketo {#sync-the-app-with-marketo}

Die Marketo Ereignisses-App funktioniert unabhängig, bis Sie Ihre Aktivität wieder mit der Marketo-Datenbank synchronisieren. Es ist am besten, so bald wie möglich nach dem letzten Check-in zu synchronisieren. Ihr Tablet muss mit dem Internet verbunden sein.

>[!CAUTION]
>
>Nach der Synchronisierung können Sie einen Check-in nicht mehr in der App rückgängig machen.

1. Öffnen Sie auf Ihrem Tablet die App und navigieren Sie zu Ihrem Ereignis.

1. Tippen Sie auf **Synchronisieren**.

   Ihr Ereignis wird mit neuen Check-ins in der Marketo-Datenbank aktualisiert. Der rote Zähler auf der Schaltfläche &quot;Synchronisieren&quot;wird gelöscht, bis Sie einen anderen Benutzer einchecken.

   Aus Sicherheitsgründen sollten Sie die Marketo Ereignisses-App beenden, nachdem Sie die Synchronisierung abgeschlossen haben.

## Arbeiten mit eingeschränktem Internetzugang {#working-with-limited-internet-access}

Einige Veranstaltungsorte haben einen lausigen Internetzugang. Sie benötigen eine gute Verbindung zu:

* Herunterladen und Installieren der App
* Anmeldung
* Ereignis auswählen
* Synchronisieren der App mit Marketo

Wenn Sie sich wegen des Internetzugangs am Veranstaltungsort Sorgen machen, können Sie sich bei der Marketo Ereignisses-App anmelden und Ihr Ereignis im Voraus auswählen, an einem Ort mit starkem Internetzugang. Auf diese Weise können Sie die App weiterhin offline verwenden. Wenn Sie dann wieder eine Internetverbindung herstellen, synchronisieren Sie diese sofort mit der Marketo-Datenbank.

>[!TIP]
>
>Wenn Sie keine Internetverbindung haben, können Sie dennoch eine neue Person für eine Person erstellen, die sich anmeldet. Es wird mit der vorhandenen Person abgeglichen, wenn Sie die App synchronisieren.

>[!NOTE]
>
>Die App meldet Sie nach acht Stunden Inaktivität automatisch ab.
