---
description: Stream erstellen - Marketo Docs - Produktdokumentation
title: Stream erstellen
hide: true
hidefromtoc: true
source-git-commit: 1022d3eaf4ee4a1686c5d8ae3168ee0197776289
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Stream erstellen {#create-a-stream}

Es gibt _viele_ Stream-Kombinationen, die Sie erstellen können. Im Folgenden finden Sie ein Beispiel, in dem der Marketingexperte den Site-Besucher fragt, ob er Produktfragen hat. Wenn ja, kann der Besucher einen Termin einplanen. Falls nein, erhält der Besucher die Möglichkeit, einer Mailing-Liste für zukünftige Korrespondenz beizutreten. Ziel ist es, einen Termin zu planen oder die E-Mail des Besuchers zu sammeln.

1. Nach [Dialogfeld erstellen](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue), klicken Sie auf **Stream-Designer** Tabulator.

   ![](assets/create-a-stream-1.png)

1. Ziehen Sie die Fragenkarte per Drag&amp;Drop.

   ![](assets/create-a-stream-2.png)

1. Geben Sie unter Chatbot-Antwort Ihre Frage an, wie Sie möchten.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke ist standardmäßig aktiviert, was die Frage zum Öffnen neben dem Chat-Symbol anzeigt, ohne dass der Besucher darauf klicken muss, um sie zu sehen.

1. Geben Sie Ihre Benutzerantworten ein und klicken Sie auf **Speichern**.

   ![](assets/create-a-stream-4.png)

1. Für &quot;Ja&quot; wollen wir einen Termin planen, so unten diese Option ziehen Sie über die Planung-Karte.

   ![](assets/create-a-stream-5.png)

1. Klicken Sie in der Spalte rechts auf **Speichern**.

   ![](assets/create-a-stream-6.png)

1. Da das ein Ziel ist, ziehen Sie die Ziellinie unter die Planung der Ernennung.

   ![](assets/create-a-stream-7.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein bestehendes Ziel) und klicken Sie auf **Speichern**.

   ![](assets/create-a-stream-8.png)

1. Für &quot;Nein&quot; wollen wir sehen, ob sie der Mailing-Liste beitreten werden, also ziehen Sie unter dieser Option über eine andere Fragenkarte.

   ![](assets/create-a-stream-9.png)

1. Geben Sie Ihre Antwort ein und fügen Sie Antwortmöglichkeiten für den Besucher hinzu. Klick **Speichern** nach Abschluss des Verfahrens.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Sie können weitere Antworten hinzufügen, indem Sie **hinzufügen**.

1. Ziehen Sie unter der Antwort &quot;Ja&quot; über die Infoerfassungs-Karte, um die E-Mail des Besuchers zu erfassen.

   ![](assets/create-a-stream-11.png)

1. Klicken Sie auf **Typ** Dropdown-Liste und wählen **E-Mail**.

   ![](assets/create-a-stream-12.png)

1. Geben Sie eine Chat-Nachricht und einen Platzhalter ein. Vergewissern Sie sich, dass das Attribut dem entsprechenden Feld in Marketo zugeordnet ist, und klicken Sie auf **Speichern**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Typ</strong></td>
     <td>Der Typ der Informationen, die Sie erfassen möchten: Telefon, Text, E-Mail.</td>
    </tr>
    <tr>
     <td><strong>Chatbot-Meldung</strong></td>
     <td>Die Meldung, die der Besucher sieht, fordert ihn auf, die Informationen bereitzustellen.</td>
    </tr>
    <tr>
     <td><strong>Platzhalter</strong></td>
     <td>Beispieltext, der dem Besucher zeigt, was er eingeben soll.</td>
    </tr>
    <tr>
     <td><strong>Antwort auf Attribut zuordnen</strong></td>
     <td>Ermöglicht es Ihnen, die Antwort des Besuchers auf das entsprechende Feld in seinem Personendatensatz in Ihrem Marketo-Abonnement zu synchronisieren.</td>
    </tr>
   </table>

1. Da das Sammeln ihrer E-Mail ein Ziel ist, ziehen Sie die Zielkarte unter &quot;Infoaufnahme&quot;.

   ![](assets/create-a-stream-14.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein bestehendes Ziel) und klicken Sie auf **Speichern**.

   ![](assets/create-a-stream-15.png)

1. Denken Sie daran, eine Antwort hinzuzufügen, wenn Sie &quot;Nein&quot; sagen. Ziehen Sie eine Nachrichtenkarte unter diese Option.

   ![](assets/create-a-stream-16.png)

1. Geben Sie Ihre Nachricht ein und klicken Sie auf **Speichern**.

   ![](assets/create-a-stream-17.png)

1. Klicken Sie zum Aktivieren des Dialogfelds auf **Veröffentlichen**.

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>Bevor Sie auf &quot;Veröffentlichen&quot;klicken, stellen Sie sicher, dass Sie [hat Ihre Zielgruppe-URL(s) eingegeben](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[Dialogfelder](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
