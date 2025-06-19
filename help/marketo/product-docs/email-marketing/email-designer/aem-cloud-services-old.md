---
title: Experience Manager-Dokument verbinden
description: Erfahren Sie, wie Sie Adobe Experience Manager Cloud Services mit Adobe Marketo Engage verbinden, damit Sie Ihre AEM-Assets nutzen können.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Adobe Experience Manager Cloud Services verbinden {#connect-adobe-experience-manager-cloud-services}

Erfahren Sie, wie Sie Ihr AEM Assets Cloud Services-Konto mit Ihrer Adobe Marketo Engage-Instanz verbinden, um Ihr AEM Asset-Repository in der Marketo Engage E-Mail-Designer nutzen zu können.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Wechseln Sie in Marketo Engage zum Bereich **Admin** und wählen Sie **Adobe Experience Manager** in der linken Navigationsstruktur aus.

SCREENSHOT

1. Klicken Sie **Bearbeiten** neben _Adobe Experience Manager Cloud Services_.

SCREENSHOT

1. Ein oder mehrere Repositorys auswählen.

SCREENSHOT

>[!NOTE]
>
>Es werden nur Repositorys aufgelistet, die derselben IMS-Organisation zugeordnet wurden wie Ihr Marketo Engage-Abonnement.

1. Sie müssen ein [Dienstanmeldeinformationszertifikat“ hinzufügen](https://experienceleague.adobe.com/de/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) um das Repository zu konfigurieren. Klicken Sie auf die Schaltfläche **+ Zertifikat hinzufügen**.

SCREENSHOT

1. Ziehen Sie Ihr Zertifikat per Drag-and-Drop (nur JSON-Datei) oder wählen Sie es von Ihrem Computer aus. Klicken Sie abschließend **Hinzufügen**.

SCREENSHOT

1. Das konfigurierte Repository wird unten zusammen mit Status und Gültigkeit angezeigt. Klicken Sie auf die Schaltfläche mit den Auslassungspunkten (**…**), um das Zertifikat anzuzeigen. Andernfalls sind Sie fertig.

SCREENSHOT

Jetzt können alle Bilder aus der Digital Asset Management-Bibliothek in diesem Repository über die Marketo Engage E-Mail-Designer aufgerufen werden.

>[!MORELIKETHIS]
>
>[Arbeiten mit Experience Manager-Assets](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
