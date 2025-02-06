---
title: Experience Manager-Dokument verbinden
description: Erfahren Sie, wie Sie Adobe Experience Manager Cloud Service mit Adobe Marketo Engage verbinden, damit Sie Ihre AEM-Assets nutzen können.
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Adobe Experience Manager Cloud Service verbinden {#connect-adobe-experience-manager-cloud-services}

Erfahren Sie, wie Sie Ihr AEM Assets Cloud Service-Konto mit Ihrer Adobe Marketo Engage-Instanz verbinden, um Ihr AEM Asset-Repository in der Marketo Engage-E-Mail-Designer nutzen zu können.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Wechseln Sie in Marketo Engage zum Bereich **Admin** und wählen Sie **Adobe Experience Manager** in der linken Navigationsstruktur aus.

   ![Wählen Sie Adobe Experience Manager im Administratorbereich aus](assets/connect-adobe-experience-manager-cloud-services-1.png){width="800"}

1. Klicken Sie **Bearbeiten** neben _Adobe Experience Manager Cloud Service_.

   ![KLICKEN SIE AUF BEARBEITEN](assets/connect-adobe-experience-manager-cloud-services-2.png){width="400"}

1. Ein oder mehrere Repositorys auswählen.

   ![Repository auswählen](assets/connect-adobe-experience-manager-cloud-services-3.png){width="800"}

   >[!NOTE]
   >
   >Es werden nur Repositorys aufgelistet, die derselben IMS-Organisation zugeordnet wurden wie Ihr Marketo Engage-Abonnement.

1. Sie müssen ein [Dienstanmeldeinformationszertifikat“ hinzufügen](https://experienceleague.adobe.com/de/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) um das Repository zu konfigurieren. Klicken Sie auf die Schaltfläche **+ Zertifikat hinzufügen**.

   ![Zertifikat hinzufügen](assets/connect-adobe-experience-manager-cloud-services-4.png){width="800"}

1. Ziehen Sie Ihr Zertifikat per Drag-and-Drop (nur JSON-Datei) oder wählen Sie es von Ihrem Computer aus. Klicken Sie abschließend **Hinzufügen**.

   ![Suchen Sie das Zertifikat auf Ihrem Computer](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

1. Das konfigurierte Repository wird unten zusammen mit Status und Gültigkeit angezeigt. Klicken Sie auf die Schaltfläche mit den Auslassungspunkten (**…**), um das Zertifikat anzuzeigen. Andernfalls sind Sie fertig.

   ![Das Zertifikat wurde hinzugefügt](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

Jetzt können alle Bilder aus der Digital Asset Management-Bibliothek in diesem Repository über die Marketo Engage-E-Mail-Designer aufgerufen werden.

>[!MORELIKETHIS]
>
>[Arbeiten mit Experience Manager-Assets](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
