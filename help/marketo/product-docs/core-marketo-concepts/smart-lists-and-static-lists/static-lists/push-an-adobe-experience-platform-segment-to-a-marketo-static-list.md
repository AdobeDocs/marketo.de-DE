---
description: Senden eines Adobe Experience Platform-Segments an eine statische Marketo-Liste - Marketo-Dokumente - Produktdokumentation
title: Adobe Experience Platform-Segment in eine statische Marketo-Liste pushen
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Adobe Experience Platform-Segment in eine statische Marketo-Liste pushen {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Mit dieser Funktion können Sie Segmente, die sich in Ihrer Adobe Experience Platform befinden, in Form einer statischen Liste an Marketo übergeben.

>[!PREREQUISITES]
>
>* [API-Rolle bearbeiten](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) , um sicherzustellen, dass **Lese-/Schreibperson** -Berechtigung (zu finden unter der Dropdown-Liste Access API ).
>* [Erstellen eines API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) in Marketo.
>* Navigieren Sie zu **Admin** > **Startpunkt**. Suchen Sie den Namen der soeben erstellten Rolle und klicken Sie auf **Details anzeigen**. Kopieren und speichern Sie die Informationen in **Client-ID** und **Client Secret**, da Sie es für Schritt 7 benötigen könnten.
>* Erstellen Sie in Marketo eine statische Liste oder suchen und wählen Sie eine bereits erstellte Liste aus. Sie werden ihre Kennung benötigen.

1. Anmelden bei [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Klicken Sie auf das Rastersymbol und wählen Sie **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Klicken Sie im linken Navigationsbereich auf **Ziele**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Klicken **Katalog**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Suchen Sie die Kachel Marketo Engage und klicken Sie auf **Aktivieren**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Klicken **Neues Ziel konfigurieren**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Wählen Sie unter Kontotyp die Optionsschaltfläche Vorhandenes oder Neues Konto aus (in diesem Beispiel wählen wir **Vorhandenes Konto**). Klicken Sie auf das Symbol Konto auswählen .

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Wenn Sie Neues Konto auswählen, können Sie Ihre Munchkin-ID finden, indem Sie **Admin** > **Munchkin** (ist auch Teil Ihrer Marketo-URL, nachdem Sie angemeldet sind). Client-ID/Geheimnis , die Sie benötigen, um die Voraussetzungen oben in diesem Artikel zu erfüllen.

1. Wählen Sie das Zielkonto aus und klicken Sie auf **Auswählen**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Ziel eingeben **Name** und eine optionale Beschreibung. Klicken Sie auf das Dropdown-Menü &quot;Personenerstellung&quot;und wählen Sie &quot;Vorhandene Marketo-Personen abgleichen und Fehlende Personen in Marketo erstellen&quot;. _oder_ &quot;Nur vorhandene Marketo-Personen abgleichen&quot;(in diesem Beispiel wählen wir die erste aus). Sie müssen auch eine **Arbeitsbereich**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Nur vorhandene Marketo-Personen abgleichen&quot;auswählen, müssen Sie nur die E-Mail und/oder die ECID zuordnen, damit Sie die Schritte 13-16 überspringen können.

1. Dieser Abschnitt ist optional. Klicken **Erstellen** überspringen.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Wählen Sie das von Ihnen erstellte Ziel aus und klicken Sie auf **Nächste**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Wählen Sie das Segment aus, das Sie an Marketo senden möchten, und klicken Sie auf **Nächste**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Wenn Sie mehrere Segmente auswählen, müssen Sie jedes Segment einer angegebenen statischen Liste auf der Registerkarte Segmentplan zuordnen.

   >[!IMPORTANT]
   >
   >Nachdem ein Segment zum ersten Mal für das Marketo-Ziel aktiviert wurde, kann das Aufstocken von Profilen, die bereits vor der Marketo-Zielaktivierung im Segment vorhanden waren, **bis zu 24 Stunden**. Künftig werden jedes Mal, wenn Profile zum Segment hinzugefügt werden, sie sofort zu Marketo hinzugefügt.

1. Klicken **Neue Zuordnung hinzufügen**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Klicken Sie auf das Zuordnungssymbol.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Wählen Sie die gewünschten Attribute aus und klicken Sie auf **Auswählen**. In diesem Beispiel wählen wir Vorname, Nachname und E-Mail-Adresse.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >Sie können Attribute von Experience Platform zu allen Attributen zuordnen, auf die Ihr Unternehmen in Marketo Engage Zugriff hat. Verwenden Sie die [API-Anfrage beschreiben](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} , um Attributfelder abzurufen, auf die Ihr Unternehmen Zugriff hat.

1. Ordnen Sie Nachname und Firmenname zu, indem Sie auf **Neue Zuordnung hinzufügen** Wiederholen und Wiederholen von Schritt 15 zweimal, wählen Sie **lastName** und dann **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Jetzt ist es Zeit, die E-Mail-Adresse zuzuordnen. Klicken **Neue Zuordnung hinzufügen** erneut.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Klicken Sie auf das Zuordnungssymbol.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Klicken Sie auf die Optionsschaltfläche Identitäts-Namespace auswählen . Wählen Sie  **Email** Klicken Sie auf **Auswählen**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Zuordnen von E-Mail und/oder ECID aus der **Identitäts-Namespace** -Registerkarte ist die wichtigste Maßnahme, um sicherzustellen, dass die Person in Marketo übereinstimmt. Die Zuordnung von E-Mail stellt die höchste Übereinstimmungsrate sicher.

1. Jetzt ist es an der Zeit, die Quellfelder auszuwählen. Klicken Sie für E-Mails auf das Cursorsymbol.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Klicken Sie auf die Optionsschaltfläche Identitäts-Namespace auswählen und wählen Sie **Email** Klicken Sie auf **Auswählen**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Um das Quellfeld Unternehmensname auszuwählen, klicken Sie auf das Cursorsymbol in der Zeile.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Lassen Sie die Optionsschaltfläche Attribute auswählen aktiviert. Suchen Sie nach &quot;company&quot;und wählen Sie **companyName** Klicken Sie auf **Auswählen**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Ordnen Sie die Quellfelder für Nachname und Vorname zu, indem Sie auf das Cursorsymbol für jeden Cursor klicken und Schritt 23 zweimal wiederholen, indem Sie auswählen **lastName** und dann **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Klicken **Nächste**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Überprüfen Sie Ihre Änderungen und klicken Sie auf **Beenden**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
