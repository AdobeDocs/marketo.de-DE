---
description: Stream Designer - Marketo-Dokumente - Produktdokumentation
title: Entwerferin bzw. Entwerfer des Streams
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: ea9e02d9ad52991757f137c7c2b549b98f139ba5
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 2%

---

# Entwerferin bzw. Entwerfer des Streams {#stream-designer}

Es gibt _many_ Stream-Kombinationen möglich. Dieser Artikel enthält ein Beispiel, in dem der Marketing-Experte den Site-Besucher fragt, ob er Produktfragen hat. Falls ja, kann der Besucher einen Termin planen. Ist dies nicht der Fall, erhält der Besucher die Möglichkeit, sich einer Mailingliste für die künftige Korrespondenz anzuschließen. Ihnen wird auch eine kostenlose PDF angeboten. Das ultimative Ziel besteht darin, entweder einen Termin zu planen oder die E-Mail-Adresse des Besuchers zu erfassen.

>[!PREREQUISITES]
>
>Bevor Sie die Dokumentkarte verwenden können, müssen Sie zunächst [einrichten](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} in Ihrem Adobe-Konto.

## Designer-Karten streamen {#stream-designer-cards}

Der Stream-Designer enthält mehrere Karten, die Sie hinzufügen können, um die Chat-Konversation zu gestalten.

<table>
 <tr>
  <td><strong>Nachricht</strong></td>
  <td>Verwenden Sie, wenn Sie eine Aussage ohne Antwort erforderlich machen möchten (z. B.: "Hi! Mit dem Code SAVE25" sind alle Artikel heute um 25 % billiger.
</td>
 </tr>
 <tr>
  <td><strong>Frage</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie eine Multiple-Choice-Frage stellen möchten, von der Sie die verfügbaren Antworten erhalten (z. B.: Wofür sind Sie interessiert? Antworten = SUV, Compact, Truck usw.).</td>
 </tr>
 <tr>
  <td><strong>Dokument</strong></td>
  <td>Ermöglicht das Einbetten von PDF-Dokumenten in Dialogfelder und das Verfolgen der Aktivität von Besuchern zur Dokumenteninteraktion (Anzahl der angezeigten-Seiten, Download des Dokuments und/oder verwendete Suchbegriffe).</td>
 </tr>
 <tr>
  <td><strong>Informationserfassung</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie Informationen erfassen möchten. Die drei Felder, aus denen Sie wählen können, sind E-Mail-Adresse, Telefonnummer und Text (mit denen der Besucher eine eigene Nachricht schreiben kann).</td>
 </tr>
 <tr>
  <td><strong>Terminplaner</strong></td>
  <td>Bietet dem Besucher einen Kalender der verfügbaren Daten, um eine Weiterverfolgung zu planen. Die Verfügbarkeit eines Kalenders spiegelt <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">der nächste Agent in Zeilen</a>.</td>
 </tr>
 <tr>
  <td><strong>Ziel</strong></td>
  <td>Dies ist die einzige Karte, die die Besucher nicht sehen werden. Es liegt an Ihnen zu bestimmen, an welchem Punkt ein Ziel innerhalb des bestimmten Chat erreicht wird (z. B.: Wenn das Sammeln der E-Mail des Besuchers Ihr Ziel ist, platzieren Sie die Zielkarte unmittelbar nach der Informationserfassung im Stream).</td>
 </tr>
</table>

## Stream-Designer-Symbole {#stream-designer-icons}

In der rechten oberen Ecke des Stream-Designers sehen Sie eine Handvoll Symbole. Hier ist, was sie tun.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Fügt ein Raster zum Hintergrund für diejenigen hinzu, die diese Ansicht bevorzugen</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Vergrößert die Ansicht und erstellt größere Karten</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Verkleinert die Ansicht und erstellt kleinere Karten</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Öffnet ein Fenster, in dem Sie Ihren Chat testen können (drücken Sie zum Schließen denselben Knopf)</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Ordnet alle Karten in Ihrem Stream an</td>
 </tr>
</table>

## Erstellen eines Streams {#create-a-stream}

1. Nachdem Sie [Dialogfeld erstellt](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}, klicken Sie auf die **Stream-Designer** Registerkarte.

   ![](assets/stream-designer-6.png)

1. Ziehen Sie die Fragenkarte per Drag-and-Drop.

   ![](assets/stream-designer-7.png)

1. Geben Sie unter &quot;Chatbot-Antwort&quot;Ihre Frage an, wie Sie möchten.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Sie können das Erlebnis für bekannte Chat-Besucher mit Token personalisieren (z. B.: Hallo `{{lead.leadFirstName:""}}`). Klicken Sie einfach auf das Symbol mit geschweiften Klammern rechts und wählen Sie Ihre Auswahl aus. Fügen Sie einen Standardwert zwischen den Anführungszeichen hinzu, wenn anonyme Besucher etwas Allgemeines sehen sollen (z. B.: Hallo `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke ist standardmäßig auf ein gesetzt, wodurch die öffnende Frage neben dem Chat-Symbol angezeigt wird, ohne dass der Besucher darauf klicken muss, um sie zu sehen. Poke ist nur auf der ersten Karte in der Konversation verfügbar.

1. Geben Sie Ihre Benutzerantworten ein und klicken Sie auf **Speichern**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Gespeicherte Werte bearbeiten** ist ein optionaler Schritt für diejenigen, die einen anderen Wert in der Datenbank speichern möchten als das, was Besuchern im Chat-Bot für zugeordnete Attribute in der Fragekarte angezeigt wird (z. B.: Besucher sieht &quot;Suchmaschinenoptimierung&quot;, speichern Sie diesen Wert als &quot;SEO&quot;).

1. Für &quot;Ja&quot; möchten wir einen Termin planen. Ziehen Sie daher unterhalb dieser Option über die Karte Terminplaner .

   ![](assets/stream-designer-10.png)

1. Klicken Sie in der Spalte rechts auf **Speichern**.

   ![](assets/stream-designer-11.png)

1. Da dies ein Ziel ist, ziehen Sie die Zielkarte unter die Terminplaner.

   ![](assets/stream-designer-12.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein vorhandenes aus) und klicken Sie auf **Speichern**.

   ![](assets/stream-designer-13.png)

1. Für &quot;Nein&quot; möchten wir sehen, ob sie der Mailingliste beitreten, also unterhalb dieser Option ziehen Sie über eine andere Fragekarte.

   ![](assets/stream-designer-14.png)

1. Geben Sie Ihre Antwort ein und fügen Sie Antwortoptionen für den Besucher hinzu. Klicks **Speichern** wann geschehen.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Sie können weitere Antworten hinzufügen, indem Sie **Antwort hinzufügen**.

1. Ziehen Sie unter der Antwort &quot;Ja&quot;über die Karte &quot;Informationserfassung&quot;, damit Sie die E-Mail des Besuchers erfassen können.

   ![](assets/stream-designer-16.png)

1. Klicken Sie auf **Typ** und wählen Sie **Email**.

   ![](assets/stream-designer-17.png)

1. Geben Sie eine Chat-Bot-Nachricht und einen Platzhalter ein. Stellen Sie sicher, dass das Attribut dem entsprechenden Feld in Marketo zugeordnet ist, und klicken Sie auf **Speichern**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>Typ</strong></td>
     <td>Der Informationstyp, den Sie erfassen möchten: Telefon, Text, E-Mail.</td>
    </tr>
    <tr>
     <td><strong>Chatbot-Nachricht</strong></td>
     <td>Die Meldung, die der Besucher sieht und ihn auffordert, die Informationen anzugeben.</td>
    </tr>
    <tr>
     <td><strong>Platzhalter</strong></td>
     <td>Beispieltext, der dem Besucher dabei hilft, zu sehen, was er eingeben soll.</td>
    </tr>
    <tr>
     <td><strong>Antwort einem Attribut zuordnen</strong></td>
     <td>Hiermit können Sie die Antwort des Besuchers mit dem entsprechenden Feld in seinem Personendatensatz in Ihrem Marketo-Abonnement synchronisieren.</td>
    </tr>
   </table>

1. Da das Sammeln ihrer E-Mail ein Ziel ist, ziehen Sie die Zielkarte unter &quot;Informationserfassung&quot;.

   ![](assets/stream-designer-19.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein vorhandenes aus) und klicken Sie auf **Speichern**.

   ![](assets/stream-designer-20.png)

1. Denken Sie daran, eine Antwort hinzuzufügen, wenn Sie &quot;Nein&quot;sagen. Eine Option besteht darin, eine Nachrichten-Karte unten zu ziehen und &quot;Danke trotzdem&quot; zu sagen. Aber in diesem Beispiel stellen wir ihnen stattdessen ein kostenloses PDF-Dokument zur Verfügung.

   ![](assets/stream-designer-21.png)

1. In diesem Beispiel erstellen wir ein neues Dokument. Geben Sie einen Namen ein, geben Sie die URL für die PDF ein, die Sie bereits gehostet haben, und klicken Sie auf **Speichern**.

   ![](assets/stream-designer-22.png)

1. Wählen Sie die **Vorschau** Umschalten auf Vorschau des Dialogfelds.

   ![](assets/stream-designer-23.png)

1. Wenn Sie bereit sind, Ihr Dialogfeld zu aktivieren, klicken Sie auf **Veröffentlichen**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Stellen Sie vor dem Klicken auf Veröffentlichen sicher, dass Sie [Ihre Ziel-URL(s) eingegeben haben](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Erstellen eines Dialogfelds](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Zielgruppenkriterien](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* [Berichte](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [Verwenden der Dokumentkarte](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}

