---
unique-page-id: 42762511
description: Einrichten der Adobe-Organisationszuordnung - Marketo-Dokumente - Produktdokumentation
title: Einrichten der Adobe-Organisationszuordnung
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: 492f21f090dc2478271172cf7db470e16f202366
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Einrichten der Adobe-Organisationszuordnung {#set-up-adobe-organization-mapping}

Um eine Synchronisierung mit Adobe Apps wie Audience Manager, dem Marketo-Connector der B2B-CDP-Datei, Dynamic Chat usw. herzustellen, müssen Sie zunächst Ihre Adobe IMS-Org-Anmeldedaten in Marketo eingeben.

>[!NOTE]
>
>Eine HIPAA-bereite Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.

>[!CAUTION]
>
>Für Kunden, die in die Adobe Business Platform und Identity Management integriert sind, wird die mit dem Abonnement verknüpfte Organisations-ID bereits ausgefüllt und ist ein schreibgeschütztes Feld.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Klicken Sie unter &quot;Integration&quot;auf **Adobe-Organisationszuordnung**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicken **Bearbeiten**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Geben Sie Ihre Adobe IMS-Organisations-ID ein (erfahren Sie, wie Sie [here](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) und klicken Sie auf **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicken **Bestätigen**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicken **Schließen**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Aus Sicherheitsgründen müssen Sie Org-Admin für die Adobe-Organisation sein, der Sie eine Zuordnung zuweisen möchten. Wenn du nicht bist, schlägt die Aktion fehl. Außerdem müssen der Adobe-Benutzer und der Marketo-Benutzer bei der Anmeldung dieselbe E-Mail-Adresse verwenden.

1. Wenn du _not_ bereits angemeldet ist, wird ein Popup in einer neuen Registerkarte/einem neuen Fenster angezeigt. Melden Sie sich bei Ihrer Adobe-Organisation an (durch diese Aktion wird der Organisationszugriff überprüft).

Und das ist es! Sie können jetzt [Zielgruppendaten freigeben](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} zu oder [Zielgruppe synchronisieren](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target=&quot;_blank&quot;} aus Adobe Experience Cloud.
