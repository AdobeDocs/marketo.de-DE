---
unique-page-id: 2949839
description: Überprüfen Sie Personen in Ihr Ereignis auf Ihrem Tablet - Marketo-Dokumente - Produktdokumentation
title: Personen in Ihr Ereignis einchecken über Ihr Tablet
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Personen in Ihr Ereignis einchecken über Ihr Tablet {#check-people-into-your-event-from-your-tablet}

Wenn Personen bei Ihrer Veranstaltung angezeigt werden, finden Sie deren Informationen in der App. Nach dem Einchecken werden sie bei der Synchronisierung mit Marketo zum Status &quot;Beendet&quot;beworben.

>[!IMPORTANT]
>
>Am 2. Oktober 2023 hat Adobe die Marketo Events App aus allen App Stores entfernt. Wenn Sie die App bereits auf Ihrem Tablet/Mobilgerät installiert haben, können Sie sie vorerst weiter verwenden. Sobald Ihre Marketo Engage-Instanz zur Authentifizierung von Marketo zu Adobe Identity migriert wurde, können Sie nicht mehr auf die App zugreifen. [Weitere Infos](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}.

Die App funktioniert sowohl für [!DNL iPad] als auch für [!DNL Android] gleich, mit Ausnahme kleiner Unterschiede bei Layout und Design.

>[!PREREQUISITES]
>
>* Erstellen Sie ein Ereignis in Marketo und fügen Sie es mit eingeladenen und registrierten Personen ein.

## Einchecken registrierter Gäste {#check-in-registered-guests}

1. Tippen Sie auf das App-Symbol auf Ihrem [!DNL iPad]- oder [!DNL Android]-Tablet.

1. Tippen Sie auf **[!UICONTROL Anmelden]** , um die Marketo Event-App zu starten.

   ![](assets/1.jpg)

1. Geben Sie Ihren Marketo-Benutzernamen und Ihr Kennwort ein und klicken Sie auf **[!UICONTROL Anmelden]**.

   >[!NOTE]
   >
   >Sie müssen über eine Rolle mit Zugriff auf die Datenbank verfügen, um Personen in der App anzuzeigen.

1. Wählen Sie ein **[!UICONTROL Ereignis]** aus.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Es werden nur Veranstaltungsprogramme (mit Ausnahme von Webinaren) angezeigt, die eine Woche vor und eine Woche nach dem heutigen Datum geplant sind.

1. Suchen Sie auf dem Startbildschirm nach registrierten Gästen. Um eine Person in der Liste zu finden, können Sie:

   * Scrollen Sie nach einem Namen
   * Geben Sie einen Namen in das Suchfeld ein
   * Wechseln Sie zu einem bestimmten ersten Buchstaben des Nachnamens, indem Sie auf der rechten Seite der Liste auf den entsprechenden Buchstaben tippen.

   >[!NOTE]
   >
   >Der Prozess ist bei [!DNL iPad] und [!DNL Android] identisch, aber die Bildschirme unterscheiden sich, und die Elemente können sich an verschiedenen Positionen befinden. Dieser Artikel enthält die [!DNL iPad] -Benutzeroberfläche. Vergleichen Sie den Bildschirm [!DNL Android] in diesem Abschnitt zur Referenz.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Tippen Sie auf den ausgewählten Namen und tippen Sie im Personendatensatz auf **[!UICONTROL Einchecken]**.

   ![](assets/img-0068-35-hands.png)

Der Gast hat jetzt den Status &quot;Geplant&quot;und erhält ein Häkchen. Der Personendatensatz wird bei der Synchronisierung mit Marketo aktualisiert. Der rote Zähler auf der Schaltfläche Synchronisieren wird erhöht und zeigt die Anzahl der Check-ins seit der letzten Synchronisation mit Marketo an. Die Schaltfläche &quot;Synchronisieren&quot;sieht anders aus und befindet sich an einem anderen Speicherort für [!DNL iPad] und [!DNL Android]:

**[!DNL iPad]**

![](assets/image2016-4-12-14-3a25-3a13.png)

**[!DNL Android]**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Wenn eine Person eingeladen, sich aber nicht registriert hat, können Sie nach dem Namen suchen, indem Sie auf **[!UICONTROL Auf Server suchen]** klicken, direkt unter dem Suchfeld. Der Status &quot;Eingeladen&quot;ändert sich für das Ereignis in **[!UICONTROL Bewirkt]** .

## Erstellen einer neuen Person auf der Registerkarte {#create-a-new-person-on-the-tablet}

Sie können in Ihrer Marketo-Datenbank nicht vorhandene Gäste manuell hinzufügen. Sie werden automatisch eingecheckt und Ihrer Datenbank hinzugefügt, wenn Sie mit Marketo synchronisieren.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Füllen Sie so viele grundlegende Informationsfelder wie möglich aus und tippen Sie auf **[!UICONTROL Fertig]**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Sie können nur die vorhandenen Felder verwenden. Sie können keine benutzerdefinierten erstellen.

   >[!CAUTION]
   >
   >Überprüfen Sie die E-Mail-Adresse. Andere Felder können später korrigiert werden, aber die E-Mail-Adresse ist die primäre Methode, den Gast zu kontaktieren.

Die neue Person wird als bei Ihrem Ereignis eingecheckt und bei der Synchronisierung mit Marketo der Marketo-Datenbank mit dem Status &quot;Geplant&quot;hinzugefügt.

## Ein Einchecken umkehren {#reverse-a-check-in}

Wenn Sie versehentlich eine Person eingecheckt haben, _bevor Sie die Synchronisation mit Marketo_ durchgeführt haben, können Sie den Status &quot;Beendet&quot;umkehren.

1. Tippen Sie auf den Namen in der Liste und im Personendatensatz auf **[!UICONTROL Rückgängig]**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Alles repariert!

## Bearbeiten eines Personendatensatzes beim Einchecken {#edit-a-person-record-at-check-in}

Sie können Gastinformationen direkt bei der Veranstaltung hinzufügen und ändern!

1. Tippen Sie auf den Namen in der Personenliste und dann auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Bearbeiten und fügen Sie Informationen zu den Feldern hinzu und tippen Sie dann auf **[!UICONTROL Fertig]**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >In [!DNL Android] kann die Schaltfläche **[!UICONTROL Fertig]** ausgeblendet sein. Scrollen Sie nach unten, um ihn zu finden.

Die Informationen werden aktualisiert, wenn Sie die App mit Marketo synchronisieren.

## Synchronisieren der App mit Marketo {#sync-the-app-with-marketo}

Die Marketo Events-App funktioniert unabhängig, bis Sie Ihre Aktivität wieder mit der Marketo-Datenbank synchronisieren. Es ist am besten, so bald wie möglich nach dem letzten Einchecken zu synchronisieren. Ihr Tablet muss mit dem Internet verbunden sein.

>[!CAUTION]
>
>Nach der Synchronisierung können Sie ein Einchecken aus der App nicht rückgängig machen.

1. Öffnen Sie auf Ihrem Tablet die App und navigieren Sie zu Ihrem Ereignis.

1. Tippen Sie auf **[!UICONTROL Synchronisieren]**.

   Ihr Ereignis wird mit neuen Check-ins in der Marketo-Datenbank aktualisiert. Der rote Zähler auf der Synchronisierungsschaltfläche wird gelöscht, bis Sie einen anderen Benutzer einchecken.

   Aus Sicherheitsgründen sollten Sie die Marketo Events-App beenden, nachdem Sie die Synchronisierung abgeschlossen haben.

## Arbeiten mit eingeschränktem Internetzugang {#working-with-limited-internet-access}

Einige Veranstaltungsorte haben einen lausigen Internetzugang. Sie benötigen eine gute Verbindung zu:

* Herunterladen und Installieren des Programms
* Anmeldung
* Ereignis auswählen
* Synchronisieren der App mit Marketo

Wenn Sie sich wegen des Internetzugangs am Veranstaltungsort Sorgen machen, können Sie sich bei der Marketo Events-App anmelden und Ihre Veranstaltung vorab an einem Ort mit starkem Internetzugang auswählen. Auf diese Weise können Sie die App weiterhin offline verwenden. Wenn Sie dann wieder eine Internetverbindung herstellen, synchronisieren Sie sofort mit der Marketo-Datenbank.

>[!TIP]
>
>Wenn Sie keine Internetverbindung haben, können Sie noch eine neue Person für eine Person erstellen, die eincheckt. Sie stimmen bei der Synchronisierung der App mit der vorhandenen Person überein.

>[!NOTE]
>
>Die App meldet Sie nach acht Stunden Inaktivität automatisch ab.
