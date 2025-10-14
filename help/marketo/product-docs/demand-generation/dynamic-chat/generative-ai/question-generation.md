---
description: Fragengenerierung - Marketo-Dokumente - Produktdokumentation
title: Generierung von Fragen
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 3%

---

# Generierung von Fragen {#question-generation}

Zeigen Sie alle Ihre Aufgaben und deren relevante Details an, z. B. den Zeitpunkt, zu dem sie generiert wurden, die Gesamtzahl der Fragen, den Genehmigungsstatus und mehr.

## Fragen generieren {#generate-questions}

1. Klicken Sie unter Generative KI auf **[!UICONTROL Unterstützte Antworten]**.

   ![](assets/question-generation-1.png)

1. Klicken Sie **[!UICONTROL Fragen generieren]**.

   ![](assets/question-generation-2.png)

1. Geben Sie der Aufgabe einen Namen und eine Quell-URL (bis zu 10), aus der der gesamte Inhalt extrahiert wird. Geben Sie die gewünschten Themen/Keywords ein und drücken Sie die Eingabetaste auf der Tastatur. Klicken Sie abschließend auf **[!UICONTROL Generieren]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Um sicherzustellen, dass Marketo Engage Inhalte aus den bereitgestellten URLs abkratzen kann, müssen zunächst mehrere IP-Adressen auf die Zulassungsliste gesetzt werden. [Einzelheiten finden Sie unten](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >Sites/Seiten müssen öffentlich sein (d. h. sie dürfen nicht hinter einem Login versteckt sein), damit ihre Informationen entfernt werden können.

1. Je nach Inhalt kann die Erstellung von Fragen und Antworten bis zu 30 Minuten dauern. Klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Klicken Sie auf Aktualisieren , um den neuesten Status Ihrer Fragegenerierung anzuzeigen.

   ![](assets/question-generation-5.png)

## Fragen und Antworten herunterladen {#download-questions-and-responses}

>[!NOTE]
>
>Die generierten Fragen und Antworten können auch in der [Antwortbibliothek“ angezeigt &#x200B;](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Suchen Sie die gewünschte Aufgabe und klicken Sie auf das Download-Symbol neben ihrem Namen.

   ![](assets/question-generation-6.png)

1. Suchen Sie den Ordner Downloads in Ihrem Browser und wählen Sie die Datei aus. Dies kann je nach verwendetem Browser unterschiedlich aussehen.

   ![](assets/question-generation-7.png)

1. In der Excel-Datei zeigt **[!DNL Task details]** genau das, verschiedene Details über die Aufgabe, einschließlich Anweisungen zum Hinzufügen/Bearbeiten von Fragen und/oder Antworten.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Wenn Sie sich entscheiden, Fragen und/oder Antworten massenweise hinzuzufügen/zu bearbeiten, [erfahren Sie hier, wie Sie sie erneut hochladen können](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Die Registerkarte **[!DNL Q&Rs]** enthält zusätzliche Details, einschließlich der generierten Fragen und Antworten.

   ![](assets/question-generation-9.png)

## IP-Adressen für die Zulassungsliste {#ip-addresses-to-allowlist}

Um die Extraktion von Inhalten aus Ihren Web-URLs während der Generierung von Fragen und Antworten zu ermöglichen, suchen Sie bitte Ihre Region unten und stellen Sie sicher, dass die damit verbundene IP-Adresse von Ihrem Web-Team auf die Zulassungsliste gesetzt wird.

<table width="450">
<thead>
  <tr>
    <th>Nordamerika</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
