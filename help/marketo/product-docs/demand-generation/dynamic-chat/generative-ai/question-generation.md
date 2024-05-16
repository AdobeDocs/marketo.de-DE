---
description: Fragengenerierung - Marketo-Dokumente - Produktdokumentation
title: Fragengenerierung
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 3788898496c50ebc3a5a8bf6adbd79a270024be7
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Fragengenerierung {#question-generation}

Sehen Sie sich all Ihre Aufgaben und ihre relevanten Details an, z. B. wann sie generiert wurden, die Gesamtzahl der Fragen, den Genehmigungsstatus und mehr.

## Fragen generieren {#generate-questions}

1. Klicken Sie unter Generative KI auf **[!UICONTROL Unterstützte Antworten]**.

   ![](assets/question-generation-1.png)

1. Klicks **[!UICONTROL Fragen generieren]**.

   ![](assets/question-generation-2.png)

1. Geben Sie Ihrer Aufgabe einen Namen und eine Quell-URL (bis zu 10) ein, aus der der gesamte Inhalt extrahiert wird. Geben Sie die gewünschten Themen/Keywords ein und drücken Sie die Eingabetaste auf der Tastatur. Klicken Sie abschließend auf **[!UICONTROL Erzeugen]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Um sicherzustellen, dass Marketo Engage Inhalte aus den bereitgestellten URLs löschen kann, müssen Sie zunächst mehrere IP-Adressen auf die Zulassungsliste gesetzt haben. [Weitere Informationen finden Sie unten](#ip-addresses-to-allowlist).

1. Je nach Inhalt kann die Erstellung von Fragen und Antworten bis zu 30 Minuten dauern. Klicks **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Tippen Sie auf Aktualisieren , um den neuesten Status der Fragengenerierung anzuzeigen.

   ![](assets/question-generation-5.png)

## Herunterladen von Fragen und Antworten {#download-questions-and-responses}

>[!NOTE]
>
>Die generierten Fragen und Antworten sind auch im [Reaktionsbibliothek](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Suchen Sie die gewünschte Aufgabe und klicken Sie auf das Download-Symbol neben ihrem Namen.

   ![](assets/question-generation-6.png)

1. Suchen Sie den Ordner Downloads in Ihrem Browser und wählen Sie die Datei aus. Dies kann je nach verwendetem Browser anders aussehen.

   ![](assets/question-generation-7.png)

1. In der Excel-Datei **[!DNL Task details]** zeigt genau dies, verschiedene Details zur Aufgabe, einschließlich Anweisungen zum Hinzufügen/Bearbeiten von Fragen und/oder Antworten.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Wenn Sie sich entscheiden, Fragen und/oder Antworten stapelweise hinzuzufügen/zu bearbeiten, [Hier erfahren Sie, wie Sie sie erneut hochladen.](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Die **[!DNL Q&Rs]** enthält zusätzliche Details, einschließlich der generierten Fragen und Antworten.

   ![](assets/question-generation-9.png)

## IP-Adressen in der Zulassungsliste {#ip-addresses-to-allowlist}

Um die Extraktion von Inhalten aus Ihren Web-URLs während der Generierung von Fragen und Antworten zu ermöglichen, suchen Sie Ihre Region unten und stellen Sie sicher, dass alle damit verbundenen IP-Adressen von Ihrem Web-Team auf die Zulassungsliste gesetzt werden.

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
    <td>20 10 235 188</td>
    <td>20 76 246 248</td>
    <td>20 167 0 195</td>
  </tr>
  <tr>
    <td>20 10 235 189</td>
    <td>20 76 247 92</td>
    <td>20 248 128 31</td>
  </tr>
  <tr>
    <td>20 10 235 246</td>
    <td>20 76 247 134</td>
    <td>20 167 14 48</td>
  </tr>
  <tr>
    <td>20 10 235 248</td>
    <td>20 76 247 244</td>
    <td>20 167 16 63</td>
  </tr>
  <tr>
    <td>20 10 235 255</td>
    <td>20 93 168 10</td>
    <td>20 167 19 92</td>
  </tr>
  <tr>
    <td>20 10 236 96</td>
    <td>20 93 168 44</td>
    <td>20 167 1 155</td>
  </tr>
  <tr>
    <td>20 119 144 14</td>
    <td>20 105 224 16</td>
    <td>20 211 64 11</td>
  </tr>
</tbody>
</table>
