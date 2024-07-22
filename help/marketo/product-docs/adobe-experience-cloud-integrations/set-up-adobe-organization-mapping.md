---
unique-page-id: 42762511
description: Einrichten der Adobe-Organisationszuordnung - Marketo-Dokumente - Produktdokumentation
title: Einrichten der Adobe-Organisationszuordnung
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Einrichten der Adobe-Organisationszuordnung {#set-up-adobe-organization-mapping}

Um eine Synchronisation mit Adobe-Applikationen wie Audience Manager, dem Marketo-Connector der B2B-CDP, [!DNL Dynamic Chat] usw. durchzuführen, müssen Sie zunächst Ihre Adobe IMS-Org-Anmeldeinformationen auf Marketo Engage eingeben.

>[!NOTE]
>
>* Eine HIPAA-bereite Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.
>* Damit die Integration funktioniert, müssen sich Marketo und Ihre anderen Adobe-Anwendungen in derselben Organisation befinden.

>[!IMPORTANT]
>
>Für diejenigen, die an die Adobe Business Platform und das Identity Management-System angeschlossen sind, wird die mit dem Abonnement verknüpfte Organisations-ID bereits ausgefüllt und ist ein schreibgeschütztes Feld. Die Schritte in diesem Artikel würden daher nicht gelten.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Klicken Sie unter &quot;Integration&quot;auf **[!UICONTROL Adobe-Organisationszuordnung]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Geben Sie Ihre Adobe IMS-Organisations-ID ein (erfahren Sie, wie Sie diese [hier](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"} finden) und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Aus Sicherheitsgründen müssen Sie Org-Admin für die Adobe-Organisation sein, der Sie eine Zuordnung zuweisen möchten. Wenn du nicht bist, schlägt die Aktion fehl. Außerdem müssen der Adobe-Benutzer und der Marketo-Benutzer bei der Anmeldung dieselbe E-Mail-Adresse verwenden.

1. Wenn Sie _nicht_ bereits angemeldet sind, wird ein Popup in einer neuen Registerkarte/einem neuen Fenster angezeigt. Melden Sie sich bei Ihrer Adobe-Organisation an (diese Aktion validiert den Organisationszugriff).

Und das ist es! Sie können jetzt [Zielgruppendaten ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} für eine Zielgruppe freigeben oder [ eine Zielgruppe synchronisieren](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} von Adobe Experience Cloud.
