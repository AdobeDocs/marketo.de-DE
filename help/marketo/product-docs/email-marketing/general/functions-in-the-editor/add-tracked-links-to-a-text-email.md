---
unique-page-id: 1900589
description: Erfahren Sie, wie Sie getrackte Links zu schreibgeschützten E-Mails hinzufügen. Aktivieren Sie Linktracking, damit Sie Klicks in Ihren E-Mail-Berichten messen können.
title: Hinzufügen nachverfolgter Links zu einer Text-E-Mail
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/zz5DkOWG-x3y-oq-E77xRAZtcNdmimbwKsctKSChnXM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 7%
---
# Hinzufügen nachverfolgter Links zu einer Text-E-Mail {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Erstellen einer reinen Text-E-Mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Elemente in einer E-Mail bearbeiten](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

E-Mail-Links in Textform können in Marketo nachverfolgt werden. Sehen wir uns an, wie das funktioniert.

1. Wählen Sie Ihre E-Mail aus und klicken Sie **Entwurf bearbeiten**.

1. Wählen Sie Ihre E-Mail aus und klicken Sie **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/one-9.png)

1. Doppelklicken Sie auf den bearbeitbaren Bereich, dem Sie den Link hinzufügen möchten.

   ![](assets/two-8.png)

1. Geben Sie die URL mit doppelten Klammern wie folgt ein: `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Wenn eine E-Mail vor mehr als 365 Tagen gesendet wurde **und** niemand in den letzten 180 Tagen auf einen ihrer Links geklickt hat, bereinigt Marketo Engage die Route zur URL aus unserer Datenbank, was dazu führt, dass der Link unterbrochen wird. Wenn der Link dauerhaft sein soll, verwenden Sie kein Tracking.

1. Schließen Sie den Editor und vergessen Sie nicht, den Entwurf zu genehmigen.

   ![](assets/four-6.png)

>[!NOTE]
>
>Die mktNoTok-Klassenfunktionalität funktioniert nicht mit verfolgbaren Links in Text-E-Mails. Nur für HTML-E-Mails.
