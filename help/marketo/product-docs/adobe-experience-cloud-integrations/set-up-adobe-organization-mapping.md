---
unique-page-id: 42762511
description: Einrichten der Adobe-Organisationszuordnung - Marketo-Dokumente - Produktdokumentation
title: Einrichten der Adobe-Organisationszuordnung
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 2%

---

# Einrichten der Adobe-Organisationszuordnung {#set-up-adobe-organization-mapping}

Um mit Adobe-Programmen wie Audience Manager, dem B2B CDP-Marketo-Connector, [!DNL Dynamic Chat] usw. zu synchronisieren, müssen Sie zunächst Ihre Anmeldedaten für die Adobe IMS-Organisation in Marketo Engage eingeben.

>[!NOTE]
>
>* Eine HIPAA-fähige Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.
>* Damit die Integration funktioniert, müssen Marketo und Ihre anderen Adobe-Programme sich in derselben Organisation befinden.

>[!IMPORTANT]
>
>Für diejenigen, die sich in der Adobe Business Platform und im Identity Management-System befinden, ist die mit dem Abonnement verknüpfte Organisations-ID bereits ausgefüllt und schreibgeschützt. Die in diesem Artikel beschriebenen Schritte wären daher nicht anwendbar.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Klicken Sie unter Integration auf **[!UICONTROL Adobe-Organisationszuordnung]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Geben Sie Ihre Adobe IMS-Organisations-ID ein (erfahren Sie hier[ wie Sie sie finden](https://experienceleague.adobe.com/docs/control-panel/using/faq.html?lang=de){target="_blank"} und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Aus Sicherheitsgründen müssen Sie ein Organisations-Admin für die Adobe-Organisation sein, der Sie zuordnen möchten. Ist dies nicht der Fall, schlägt die Aktion fehl. Darüber hinaus müssen Adobe-Benutzende und Marketo-Benutzende beim Anmelden dieselbe E-Mail-Adresse verwenden.

1. Wenn Sie _noch nicht_ angemeldet sind, wird ein Popup-Fenster in einer neuen Registerkarte/einem neuen Fenster angezeigt. Melden Sie sich bei Ihrer Adobe-Organisation an (dieser Vorgang validiert den Organisationszugriff).

Sie können [ Adobe Experience Cloud jetzt Zielgruppendaten ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} oder [synchronisieren](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"}.
