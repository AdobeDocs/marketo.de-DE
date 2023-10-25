---
description: Senden eines Adobe Experience Platform-Segments an eine statische Marketo-Liste - Marketo-Dokumente - Produktdokumentation
title: Adobe Experience Platform-Segment in eine statische Marketo-Liste pushen
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Adobe Experience Platform-Segment in eine statische Marketo-Liste pushen {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Mit dieser Funktion können Sie Segmente, die sich in Ihrer Adobe Experience Platform befinden, in Form einer statischen Liste auf Marketo Engage übertragen.

>[!PREREQUISITES]
>
>* [API-Rolle bearbeiten](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role){target="_blank"} , um sicherzustellen, dass **Lese-/Schreibperson** -Berechtigung (zu finden unter der Dropdown-Liste Access API ).
>* [Erstellen eines API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"} in Marketo.
>* Navigieren Sie zu **[!UICONTROL Admin]** > **[!UICONTROL Startpunkt]**. Suchen Sie den Namen der soeben erstellten Rolle und klicken Sie auf **[!UICONTROL Details anzeigen]**. Kopieren und speichern Sie die Informationen in **[!UICONTROL Client-ID]** und **[!UICONTROL Client Secret]**, da Sie es für Schritt 7 benötigen könnten.
>* Erstellen Sie in Marketo eine statische Liste oder wählen Sie eine bereits erstellte Liste aus. Sie werden ihre Kennung benötigen.

1. Anmelden bei [Adobe Experience Platform](https://experience.adobe.com/){target="_blank"}.

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Klicken Sie auf das Rastersymbol und wählen Sie **[!UICONTROL Experience Platform]**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Ziele]**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Klicks **[!UICONTROL Katalog]**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Suchen Sie die Marketo Engage-Kachel und klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Klicks **[!UICONTROL Neues Ziel konfigurieren]**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Wählen Sie unter &quot;Kontotyp&quot;die Optionsschaltfläche Vorhandenes oder Neues Konto aus (in diesem Beispiel wählen wir **[!UICONTROL Vorhandenes Konto]**). Klicken Sie auf das Symbol Konto auswählen .

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Wenn Sie Neues Konto auswählen, können Sie Ihre Munchkin-ID finden, indem Sie **[!UICONTROL Admin]** > **[!UICONTROL Munchkin]** (ist auch Teil Ihrer Marketo-URL, nachdem Sie angemeldet sind). Client-ID/Geheimnis , die Sie benötigen, um die Voraussetzungen oben in diesem Artikel zu erfüllen.

1. Wählen Sie das Zielkonto aus und klicken Sie auf **[!UICONTROL Auswählen]**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Ziel eingeben **[!UICONTROL Name]** und eine optionale Beschreibung. Klicken Sie auf das Dropdown-Menü &quot;Personenerstellung&quot;und wählen Sie &quot;Vorhandene Marketo-Personen abgleichen und Fehlende Personen in Marketo erstellen&quot;. _oder_ &quot;Nur vorhandene Marketo-Personen abgleichen&quot;(in diesem Beispiel wählen wir die erste aus). Sie müssen auch eine **[!UICONTROL Arbeitsbereich]**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Nur vorhandene Marketo-Personen abgleichen&quot;auswählen, müssen Sie nur die E-Mail und/oder die ECID zuordnen, damit Sie die Schritte 13-16 überspringen können.

1. Dieser Abschnitt ist optional. Klicks **[!UICONTROL Erstellen]** überspringen.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Wählen Sie das erstellte Ziel aus und klicken Sie auf **[!UICONTROL Nächste]**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Wählen Sie das Segment aus, das Sie an Marketo senden möchten, und klicken Sie auf **[!UICONTROL Nächste]**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Wenn Sie mehrere Segmente auswählen, müssen Sie jedes Segment einer angegebenen statischen Liste auf der Registerkarte Segmentplan zuordnen.

   >[!IMPORTANT]
   >
   >Nachdem ein Segment zum ersten Mal für das Marketo-Ziel aktiviert wurde, kann das Aufstocken von Profilen, die bereits vor der Marketo-Zielaktivierung im Segment vorhanden waren, _bis zu 24 Stunden_. Künftig werden jedes Mal, wenn Profile zum Segment hinzugefügt werden, sie sofort zu Marketo hinzugefügt.

1. Klicks **[!UICONTROL Neue Zuordnung hinzufügen]**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Klicken Sie auf das Zuordnungssymbol.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Wählen Sie die gewünschten Attribute aus und klicken Sie auf **[!UICONTROL Auswählen]**. In diesem Beispiel wählen wir Vorname, Nachname und E-Mail-Adresse.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >Sie können Attribute von Experience Platform zu jedem der Attribute zuordnen, auf die Ihr Unternehmen in Marketo Engage Zugriff hat. Verwenden Sie die [API-Anfrage beschreiben](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} , um Attributfelder abzurufen, auf die Ihr Unternehmen Zugriff hat.

1. Ordnen Sie Nachname und Firmenname zu, indem Sie auf **[!UICONTROL Neue Zuordnung hinzufügen]** Wiederholen und Schritt 15 zweimal wiederholen, wählen Sie **[!UICONTROL lastName]** und dann **[!UICONTROL companyName]**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Jetzt ist es Zeit, die E-Mail-Adresse zuzuordnen. Klicks **[!UICONTROL Neue Zuordnung hinzufügen]** erneut.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Klicken Sie auf das Zuordnungssymbol.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Klicken Sie auf die Optionsschaltfläche Identitäts-Namespace auswählen . Wählen Sie **[!UICONTROL Email]** Klicken Sie auf **[!UICONTROL Auswählen]**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Zuordnen von E-Mail und/oder ECID aus der **[!UICONTROL Identity Namespace]** -Registerkarte ist die wichtigste Maßnahme, um sicherzustellen, dass die Person in Marketo übereinstimmt. Die Zuordnung von E-Mail stellt die höchste Übereinstimmungsrate sicher.

1. Jetzt ist es an der Zeit, die Quellfelder auszuwählen. Klicken Sie für E-Mails auf das Cursorsymbol.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Klicken Sie auf die Optionsschaltfläche Identitäts-Namespace auswählen , suchen und wählen Sie **[!UICONTROL Email]** Klicken Sie auf **[!UICONTROL Auswählen]**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Um das Quellfeld Unternehmensname auszuwählen, klicken Sie auf das Cursorsymbol in der Zeile.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Lassen Sie die Optionsschaltfläche Attribute auswählen aktiviert. Suchen Sie nach &quot;company&quot;und wählen Sie **[!UICONTROL companyName]** Klicken Sie auf **[!UICONTROL Auswählen]**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Ordnen Sie die Quellfelder für Nachname und Vorname zu, indem Sie auf das Cursorsymbol für jeden Cursor klicken und Schritt 23 zweimal wiederholen, indem Sie auswählen **[!UICONTROL lastName]** und dann **[!UICONTROL firstName]**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Überprüfen Sie Ihre Änderungen und klicken Sie auf **[!UICONTROL Beenden]**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
