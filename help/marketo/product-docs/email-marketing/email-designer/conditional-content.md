---
solution: Marketo Engage
product: marketo
title: Bedingte Inhalte
description: Erfahren Sie mehr über bedingte Inhalte zum Anzeigen unterschiedlicher Inhalte nach Empfänger. Verwenden Sie Regeln in der E-Mail-Designer, um E-Mails zu personalisieren.
level: Beginner, Intermediate
feature: Email Designer
exl-id: 979ef9db-920f-466f-8c7d-e9de1ee4cf00
TQID: https://experienceleague.adobe.com/MKNaSOXiUYlnS2KNvH2rUQXqeNxvjiIr-OlbJQvtnaA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 2%

---

# Bedingte Inhalte {#conditional-content}

Mit bedingten Inhalten können Sie dynamisch steuern, welche Inhalte von welcher Zielgruppe angezeigt werden. Verwenden Sie vorhandene Segmentierungen, um anhand vordefinierter Kriterien zu bestimmen, was ein Empfänger sieht.

>[!PREREQUISITES]
>
>Mindestens eine Segmentierung [erstellt](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) und [genehmigt](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Hinzufügen bedingter Inhalte {#add-conditional-content}

1. Öffnen Sie die gewünschte E-Mail und klicken Sie auf **E-Mail-Inhalt bearbeiten**.

   ![](assets/conditional-content-1.png)

1. Wählen Sie den Inhalt aus, der bedingt sein soll (in diesem Beispiel wählen wir das Kopfzeilenbild aus). Klicken Sie auf _Symbol „Bedingten Inhalt_&quot;.

   ![](assets/conditional-content-2.png)

1. Das Markierungsfeld wird orange. Klicken Sie links auf das Symbol _Bedingung auswählen_ (![](assets/icon-select-condition.png)), um Ihre Variante zu definieren.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Wählen Sie das gewünschte Segment aus und klicken Sie auf **Auswählen**.

   ![](assets/conditional-content-4.png)

1. Klicken Sie auf _Bild bearbeiten_, um das vorhandene Bild für die Variante zu ersetzen. Quelle des neuen Bildes auswählen. In diesem Beispiel wählen wir die Bibliothek _Bilder und Dateien_ in unserem Marketo Engage-Abonnement aus.

   ![](assets/conditional-content-5.png)

1. Wählen Sie das entsprechende Bild aus und klicken Sie auf **Auswählen**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. Das neue Bild wird angezeigt. Es empfiehlt sich, die Variante umzubenennen, damit sie leichter zu erkennen ist. Klicken Sie auf die Auslassungszeichen und wählen Sie **Umbenennen**.

   >[!NOTE]
   >
   >Durch Klicken auf die Auslassungszeichen können Sie auch die definierte Bedingung der Variante anzeigen und sie duplizieren. Wenn Sie über mehr als eine Variante verfügen, wird eine Löschoption verfügbar. Wenn Sie nur eine Variante haben, können Sie sie löschen, indem Sie einfach erneut auf das Symbol _Bedingten Inhalt aktivieren_ klicken (es lautet jetzt _Bedingten Inhalt deaktivieren_ wenn Sie den Mauszeiger darüber bewegen).

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. Um weitere Varianten hinzuzufügen (optional), klicken Sie auf **Variante hinzufügen** und führen Sie dieselben Schritte aus.

   ![](assets/conditional-content-8.png)

1. Wenn Sie fertig sind, zeigt jede Variante den ausgewählten Inhalt an.

   ![](assets/conditional-content-9.gif)

1. Empfänger sehen Inhalte basierend auf den in den einzelnen Segmenten definierten Regeln. Im obigen Beispiel sieht jeder, der „Football“ auf seinem Marketo Engage-Feld _Lieblingssport_ aufgeführt hat, das Football-Image.

>[!MORELIKETHIS]
>
>* [Definieren von Segmentregeln](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Erstellen eines benutzerdefinierten Felds in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
