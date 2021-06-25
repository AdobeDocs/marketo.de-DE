---
description: Senden eines Adobe Experience Cloud-Segments an eine statische Marketo-Liste - Marketo-Dokumente - Produktdokumentation
title: Adobe Experience Cloud-Segment in eine statische Marketo-Liste pushen
hidefromtoc: true
source-git-commit: f437495fbe004177f01c57729d97d2fec1f79509
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Adobe Experience Cloud-Segment in eine statische Marketo-Liste pushen {#push-an-adobe-experience-cloud-segment-to-a-marketo-static-list}

Mit dieser Funktion können Sie Segmente, die sich in Ihrer Adobe Experience Platform befinden, in Form einer statischen Liste an Marketo übergeben.

>[!PREREQUISITES]
>
>* [Erstellen Sie einen API-](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) Benutzer in Marketo.
>* Gehen Sie dann zu **Admin** > **Launchpoint**. Suchen Sie den Namen der soeben erstellten Rolle und klicken Sie auf **Details anzeigen**. Kopieren Sie die Informationen und speichern Sie sie in **Client-ID** und **Client-Geheimnis**, da Sie sie für diese Funktion benötigen werden.


1. Melden Sie sich bei [Adobe Experience Platform](https://experience.adobe.com/) an.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-1.png)

1. Klicken Sie auf das Rastersymbol und wählen Sie **Experience Platform** aus.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-2.png)

1. Klicken Sie in der linken Navigationsleiste auf **Ziele**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-3.png)

1. Klicken Sie auf **Katalog**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-4.png)

1. Suchen Sie die Kachel Marketo Engage und klicken Sie auf **Aktivieren**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-5.png)

1. Klicken Sie unter &quot;Kontotyp&quot;auf das Optionsfeld **Neues Konto** . Geben Sie Ihre Marketo-Anmeldedaten ein und klicken Sie auf **Mit Ziel verbinden**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >Sie können Ihre Munchkin-ID finden, indem Sie **Admin** > **Munchkin** aufrufen (sie ist auch Teil Ihrer Marketo-URL, nachdem Sie angemeldet sind). Client-ID/Geheimnis , die Sie benötigen, um die Voraussetzungen oben in diesem Artikel zu erfüllen.

1. &quot;Verbunden&quot;sollte unter Ihren Anmeldedaten angezeigt werden. Klicken Sie oben rechts auf **Weiter**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-7.png)

1. Geben Sie eine **Name** und eine _optionale_ Beschreibung ein. Klicken Sie auf **Ziel erstellen**.

   >[!NOTE]
   >
   >Die Auswahl in Marketing-Aktionen ist ebenfalls optional. Marketo nutzt diese Informationen derzeit nicht, wird aber wahrscheinlich bald nutzen.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-8.png)

1. Klicken Sie auf **Next**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-9.png)

1. Wählen Sie das gewünschte Segment aus und klicken Sie auf **Weiter**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >Segmente für statische Listen sind 1:1. Wenn Sie hier mehrere Segmente auswählen, müssen Sie jedes Segment einer angegebenen statischen Liste auf der Registerkarte Segmentplan zuordnen.

1. Klicken Sie auf **Neue Zuordnung hinzufügen**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-11.png)

1. Klicken Sie auf das Cursorsymbol.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-12.png)

1. Wählen Sie das entsprechende Feld aus, das die E-Mail-Adresse enthält, die den Benutzer identifiziert. Klicken Sie abschließend auf **Wählen Sie** aus.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-13.png)

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-14.png)


   >[!NOTE]
   >
   >Das Beispiel, das wir ausgewählt haben, kann sich von Ihrer Auswahl unterscheiden.

1. Klicken Sie auf das Zuordnungssymbol.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-15.png)

1. Wählen Sie Ihr Zielfeld aus und klicken Sie auf **Wählen Sie**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-16.png)

1. Klicken Sie auf **Next**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-17.png)

1. _Erstellen Sie in Marketo_ eine statische Liste oder suchen und wählen Sie eine bereits erstellte Liste aus. Kopieren Sie die Zuordnungs-ID vom Ende der URL.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-18.png)

   >[!NOTE]
   >
   >Die besten Ergebnisse erzielen Sie, wenn die Liste, auf die Sie in Marketo verweisen, leer ist.

1. Geben Sie in Adobe Experience Platform die soeben kopierte ID ein. Wählen Sie Ihr Startdatum aus. Die Personen werden bis zum ausgewählten Enddatum kontinuierlich synchronisiert. Lassen Sie das Enddatum für eine unbegrenzte Synchronisierung leer. Klicken Sie abschließend auf **Weiter** .

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-19.png)

1. Bestätigen Sie Ihre Änderungen und klicken Sie auf **Beenden**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-20.png)
