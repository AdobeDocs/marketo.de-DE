---
unique-page-id: 7512270
description: Fügen Sie Adobe Connect als LaunchPoint-Service hinzu, damit Marketo die Registrierung und Teilnahme für Webinare verwaltet.
title: Hinzufügen von [!DNL Adobe Connect] as a [!DNL LaunchPoint] Service
exl-id: 21beb156-6674-46a8-bdc5-345fcb4bb272
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/5FY-AYMAy60RGDnuFas2QP1PexqhIMohWh8egyllFNY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f9fe6ecbdea51b51d14bd3faeef52ca9c02c831b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%
---
# Hinzufügen von [!DNL Adobe Connect] as a [!DNL LaunchPoint] Service {#add-adobe-connect-as-a-launchpoint-service}

Marketo verwaltet die Registrierung und Teilnahme an [!DNL Adobe Connect] Webinaren.

>[!PREREQUISITES]
>
>* Ein bestehendes Abonnement für [!DNL Adobe Connect] und Administratorrechte ist erforderlich. Halten Sie die folgenden Details bereit: Benutzername, Kennwort, Teilnehmerkennwort und Besprechungsordner-URL.

>[!NOTE]
>
>* **Admin-Berechtigungen erforderlich**
>* [!DNL Adobe Connect On Site] wird derzeit nicht unterstützt.

1. Klicken Sie in „Mein Marketo&quot; auf **[!UICONTROL Admin]**.

1. Wählen **[!UICONTROL unter]** die Option **[!UICONTROL LaunchPoint]** aus.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Service]** aus.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-2.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** ein. Wählen Sie in **[!UICONTROL Dropdown]** Service die Option **[!UICONTROL Adobe Connect]** aus.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-3.png)

1. Geben Sie **[!UICONTROL Benutzernamen]**, **[!UICONTROL Zugriffscode]**, **[!UICONTROL Besprechungsordner-URL]** und **[!UICONTROL Teilnehmerkennwort]** ein und klicken Sie dann auf **[!UICONTROL Erstellen]**.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-4.png)

   >[!TIP]
   >
   >Wenn Sie das Teilnehmerkennwort erstellen, wird der ausgewählte Wert in eine Abfragezeichenfolge aufgenommen, wenn die Links für das Ereignis gesendet werden. Es wird empfohlen, dass Sie es kundenfreundlich machen.

   >[!NOTE]
   >
   >Nachdem Sie sich bei Ihrem [!DNL Adobe Connect]-Konto angemeldet haben, wählen Sie die Registerkarte **[!UICONTROL Seminare]** aus. Kopieren Sie ohne ein Drilldown in ein bestimmtes Seminar die URL aus Ihrer Browser-Leiste in die Einstellung **[!UICONTROL Besprechungsordner-URL]**.

Ihr [!DNL Adobe Connect]-Service ist jetzt mit Marketo Engage synchronisiert.

>[!MORELIKETHIS]
>
>Erfahren Sie, wie Sie [ein Ereignis mit erstellen [!DNL Adobe Connect]](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-adobe-connect.md){target="_blank"}.
