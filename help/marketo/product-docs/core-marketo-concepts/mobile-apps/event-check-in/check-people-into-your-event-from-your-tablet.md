---
unique-page-id: 2949839
description: Personen von Ihrem Tablet aus in Ihre Veranstaltung einchecken - Marketo-Dokumente - Produktdokumentation
title: Personen von Ihrem Tablet aus in Ihre Veranstaltung einchecken
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Personen von Ihrem Tablet aus in Ihre Veranstaltung einchecken {#check-people-into-your-event-from-your-tablet}

Wenn Personen bei Ihrer Veranstaltung auftauchen, können Sie ihre Informationen in der App finden. Nach dem Check-in werden sie zum Status „Teilgenommen“ befördert, wenn Sie mit Marketo synchronisieren.

>[!IMPORTANT]
>
>Am 2. Oktober 2023 hat Adobe die Marketo Events App aus allen App Stores entfernt. Wenn Sie die App bereits auf Ihrem Tablet/Mobilgerät installiert haben, können Sie sie vorerst weiter verwenden. Nachdem Ihre Marketo Engage-Instanz zur Authentifizierung von Marketo zu Adobe Identity migriert wurde, können Sie nicht mehr auf die App zugreifen. [Weitere Informationen](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}.

Die App funktioniert auf beiden [!DNL iPad] und [!DNL Android] gleich, mit Ausnahme geringfügiger Layout- und Designunterschiede.

>[!PREREQUISITES]
>
>* Erstellen Sie eine Veranstaltung in Marketo und fügen Sie eingeladene und registrierte Personen hinzu.

## Einchecken registrierter Gäste {#check-in-registered-guests}

1. Tippen Sie auf das App-Symbol auf Ihrem [!DNL iPad] oder [!DNL Android] Tablet.

1. Tippen Sie auf **[!UICONTROL Anmelden]**, um die Marketo Event-App zu starten.

   ![](assets/1.jpg)

1. Geben Sie Ihren Marketo-Benutzernamen und Ihr Kennwort ein und klicken Sie auf **[!UICONTROL Anmelden]**.

   >[!NOTE]
   >
   >Sie müssen über eine Rolle mit Zugriff auf die Datenbank verfügen, um Personen in der App sehen zu können.

1. Wählen Sie ein **[!UICONTROL Ereignis]** aus.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Nur Veranstaltungsprogramme (mit Ausnahme von Webinaren), die eine Woche vor und eine Woche nach dem heutigen Datum geplant sind, werden angezeigt.

1. Suchen Sie auf dem Startbildschirm nach Registrierte Gäste. Um eine Person in der Liste zu finden, haben Sie folgende Möglichkeiten:

   * Scrollen Sie nach einem Namen
   * Einen Namen in das Suchfeld eingeben
   * Wechseln Sie zu einem bestimmten Anfangsbuchstaben des Nachnamens, indem Sie auf der rechten Seite der Liste darauf tippen

   >[!NOTE]
   >
   >Der Vorgang ist bei [!DNL iPad] und [!DNL Android] identisch, aber die Bildschirme unterscheiden sich, und die Elemente können sich an verschiedenen Orten befinden. Dieser Artikel enthält die [!DNL iPad]. Vergleichen Sie als Referenz den [!DNL Android] in diesem Abschnitt.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Tippen Sie auf den ausgewählten Namen und tippen Sie im Personendatensatz auf **[!UICONTROL Einchecken]**.

   ![](assets/img-0068-35-hands.png)

Der Gast hat jetzt den Status Anwesend und erhält ein Häkchen. Der Personendatensatz wird bei der Synchronisierung mit Marketo aktualisiert. Der rote Zähler auf der Schaltfläche Synchronisieren wird inkrementiert, um die Anzahl der Eincheckvorgänge seit der letzten Synchronisierung mit Marketo anzuzeigen. Die Schaltfläche Synchronisieren sieht anders aus und befindet sich für [!DNL iPad] und [!DNL Android] an einer anderen Stelle:

**[!DNL iPad]**

![](assets/image2016-4-12-14-3a25-3a13.png)

**[!DNL Android]**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Wenn eine Person eingeladen wurde, sich jedoch nicht registriert hat, können Sie direkt unter dem Suchfeld nach dem Namen **[!UICONTROL Auf dem Server suchen]**. Der Status der Einladung ändert sich für **[!UICONTROL Veranstaltung in]** Teilgenommen“.

## Erstellen einer neuen Person auf dem Tablet {#create-a-new-person-on-the-tablet}

Sie können Gäste, die keine vorhandenen Personen sind, manuell in Ihrer Marketo-Datenbank hinzufügen. Sie werden automatisch eingecheckt und Ihrer Datenbank hinzugefügt, wenn Sie mit Marketo synchronisieren.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Füllen Sie so viele der grundlegenden Informationsfelder wie möglich aus und tippen Sie auf **[!UICONTROL Fertig]**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Sie können nur die vorhandenen Felder verwenden. Es können keine benutzerdefinierten erstellt werden.

   >[!CAUTION]
   >
   >Überprüfen Sie die E-Mail-Adresse. Andere Felder können später korrigiert werden, aber die E-Mail-Adresse ist die primäre Methode, um den Gast zu kontaktieren.

Die neue Person wird als bei Ihrem Ereignis eingecheckt registriert und der Marketo-Datenbank mit dem Status „Anwesend“ hinzugefügt, wenn Sie mit Marketo synchronisieren.

## Umkehren eines Eincheckens {#reverse-a-check-in}

Wenn Sie versehentlich eine Person eingecheckt haben _bevor Sie mit Marketo synchronisiert haben_ können Sie den Status &quot;[!UICONTROL &quot; ].

1. Tippen Sie auf den Namen in der Liste und im Personendatensatz auf **[!UICONTROL Rückgängig]**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Alles behoben!

## Bearbeiten eines Personendatensatzes beim Einchecken {#edit-a-person-record-at-check-in}

Sie können Gastinformationen direkt bei der Veranstaltung hinzufügen und ändern!

1. Tippen Sie auf den Namen in der Personenliste und dann auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Bearbeiten Sie die Felder, fügen Sie Informationen hinzu und tippen Sie dann auf **[!UICONTROL Fertig]**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >In [!DNL Android] kann die Schaltfläche **[!UICONTROL Fertig]** ausgeblendet sein. Scrollen Sie nach unten, um es zu finden.

Die Informationen werden beim Synchronisieren der App mit Marketo aktualisiert.

## App mit Marketo synchronisieren {#sync-the-app-with-marketo}

Die Marketo Events-App funktioniert unabhängig, bis Sie Ihre Aktivität wieder mit der Marketo-Datenbank synchronisieren. Es ist am besten, so bald wie möglich nach dem letzten Check-in zu synchronisieren. Ihr Tablet muss mit dem Internet verbunden sein.

>[!CAUTION]
>
>Nach der Synchronisierung können Sie einen Check-in aus der App nicht rückgängig machen.

1. Öffnen Sie auf dem Tablet die App und navigieren Sie zu Ihrem Ereignis.

1. Tippen Sie auf **[!UICONTROL Synchronisieren]**.

   Ihr Ereignis wird mit neuen Eincheckvorgängen in der Marketo-Datenbank aktualisiert. Der rote Zähler auf der Synchronisierungsschaltfläche wird geleert, bis Sie eine andere Person einchecken.

   Aus Sicherheitsgründen sollten Sie die Marketo Events-App beenden, nachdem Sie die Synchronisierung abgeschlossen haben.

## Arbeiten mit eingeschränktem Internetzugriff {#working-with-limited-internet-access}

Manche Orte haben einen schlechten Internetzugang. Sie benötigen eine gute Verbindung zu:

* Herunterladen und Installieren der App
* Anmeldung
* Ereignis auswählen
* App mit Marketo synchronisieren

Wenn Sie sich über den Internetzugang am Veranstaltungsort Sorgen machen, sollten Sie sich bei der Marketo Events App anmelden und Ihre Veranstaltung im Voraus an einem Ort mit starkem Internetzugang auswählen. Auf diese Weise können Sie die App weiterhin offline verwenden. Wenn Sie dann wieder eine Internetverbindung herstellen, synchronisieren Sie sofort mit der Marketo-Datenbank.

>[!TIP]
>
>Wenn Sie keine Internetverbindung haben, können Sie dennoch eine neue Person für eine Person erstellen, die sich anmeldet. Sie wird mit der vorhandenen Person abgestimmt, wenn Sie die App synchronisieren.

>[!NOTE]
>
>Die App meldet Sie nach acht Stunden Inaktivität automatisch ab.
