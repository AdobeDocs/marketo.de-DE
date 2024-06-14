---
description: Stream Designer - Marketo-Dokumente - Produktdokumentation
title: Entwerferin bzw. Entwerfer des Streams
feature: Dynamic Chat
exl-id: 310b1dff-dd93-48a6-85c2-64c58494ce48
source-git-commit: 0015db05477cbb46a34e8abd4800d00c6522496f
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 2%

---

# Entwerferin bzw. Entwerfer des Streams {#stream-designer}

Es gibt _many_ Stream-Kombinationen möglich. Dieser Artikel enthält ein Beispiel, in dem der Marketing-Experte den Site-Besucher fragt, ob er Produktfragen hat. Falls ja, kann der Besucher einen Termin planen. Ist dies nicht der Fall, erhält der Besucher die Möglichkeit, sich einer Mailingliste für die künftige Korrespondenz anzuschließen. Ihnen wird auch eine kostenlose PDF angeboten. Das ultimative Ziel besteht darin, entweder einen Termin zu planen oder die E-Mail-Adresse des Besuchers zu erfassen.

>[!PREREQUISITES]
>
>Bevor Sie die Dokumentkarte verwenden können, müssen Sie zunächst [einrichten](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"} in Ihrem Adobe-Konto.

## Designer-Karten streamen {#stream-designer-cards}

Der Stream-Designer enthält mehrere Karten, die Sie hinzufügen können, um die Chat-Konversation zu gestalten.

<table>
 <tr>
  <td style="width:25%"><strong>Nachricht</strong></td>
  <td>Verwenden Sie, wenn Sie eine Aussage ohne Antwort erforderlich machen möchten (z. B.: "Hi! Mit dem Code SAVE25" sind alle Artikel heute um 25 % billiger.
</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Frage</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie eine Multiple-Choice-Frage stellen möchten, von der Sie die verfügbaren Antworten erhalten (z. B.: Wofür sind Sie interessiert? Antworten = SUV, Compact, Truck usw.).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Dokument</strong></td>
  <td>Ermöglicht das Einbetten von PDF-Dokumenten in Dialogfelder und das Verfolgen der Aktivität von Besuchern zur Dokumenteninteraktion (Anzahl der angezeigten-Seiten, Download des Dokuments und/oder verwendete Suchbegriffe).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Informationserfassung</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie Informationen erfassen möchten (z. B. Name, E-Mail-Adresse, Berufsbezeichnung usw.). Nachdem Sie ausgewählt haben, welchem Feld die Antwort zugeordnet werden soll, können Sie den Besuchertyp in der Antwort angeben oder Optionen aus einer von Ihnen festgelegten Auswahlliste auswählen (Tipp: Letzteres kann bei der Bereinigung der Datenbank helfen). Sie können auch festlegen, welche Daten Sie derzeit für die Antwort aufgelistet haben, oder die Frage vollständig überspringen, wenn Sie bereits über einen Wert für sie verfügen.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Buchung eines Meetings</strong></td>
  <td>Bietet dem Besucher einen Kalender der verfügbaren Daten, um ein Meeting zu planen. Wählen Sie die Kalenderverfügbarkeit über Round Robin, einen bestimmten Agenten oder mithilfe benutzerdefinierter Regeln. Klicks <b>Attribut hinzufügen</b> wenn Sie den Namen oder die E-Mail-Adresse des Agenten erfassen und ihn zum Personendatensatz des Chat-Besuchers für zukünftige Abfragen zuweisen möchten (Tipp: Erstellen Sie eine <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">Benutzerdefiniertes Feld</a> , um die Agenteninformationen so zuzuordnen, dass ein standardmäßiges Marketo Engage-Feld nicht überschrieben wird).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Ziel</strong></td>
  <td>Dies ist die einzige Karte, die die Besucher nicht sehen werden. Es liegt an Ihnen zu bestimmen, an welchem Punkt ein Ziel innerhalb des bestimmten Chat erreicht wird (z. B.: Wenn das Sammeln der E-Mail des Besuchers Ihr Ziel ist, platzieren Sie die Zielkarte unmittelbar nach der Informationserfassung im Stream).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Aktion*</strong></td>
  <td>Ähnlich wie ausgeblendete Felder in einem Formular können Sie mit der Aktionskarte jedes Lead- oder Firmenattribut (mit einer <a href="/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md#string">Zeichenfolgen-Datentyp</a>) mit impliziten Werten, die Sie mit einem Lead-Datensatz erfassen möchten. Sie können die Aktionskarte jederzeit in der Konversation hinzufügen und die entsprechenden Attribute mit einem Wert oder nativen Token aktualisieren, die den entsprechenden Wert automatisch ausfüllen.
  <p><i>* Diese Karte erfordert Dynamic Chat Prime. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Live-Chat</strong></td>
  <td>Verwenden Sie die Live-Chat-Karte, wenn Sie möchten, dass Besucher mit einem Live-Agenten chatten.
  <li>Die Live-Chat-Karte muss die letzte Karte im Zweig sein.</li>
  <li>Die Besucher werden an einen Agenten weitergeleitet, sobald sie diese Karte im Stream erreichen. Daher wird empfohlen, dieser Karte eine Fragenkarte mit der Frage vorzustellen, ob sie mit einem Live-Agenten chatten möchten.</li></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Generierte Antworten*</strong></td>
  <td>Erstellen Sie eine Nachricht für den Besucher, wenn er einen bestimmten Punkt in der Konversation erreicht. Stellen Sie eine Reihe von Fragen, die sie auf einmal stellen können, um Ihren gewünschten wichtigen Leistungsindikator zu erreichen.
  <p><i>* Diese Karte erfordert Dynamic Chat Prime. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Bedingte Verzweigung</strong></td>
  <td>Erstellen Sie Verzweigungen in Ihrem Dialogfeld basierend auf unterschiedlichen Bedingungen. Unterschiedliche Inhalte für verschiedene Personen im selben Dialogfeld basierend auf Lead- und Firmenattributen in Marketo Engage präsentieren.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Konversationsfluss</strong></td>
  <td>Mithilfe der Karte Konversionsfluss können Sie mehrere Schritte in einem Fluss innerhalb Ihrer Dialoge optimieren.</td>
 </tr>
</table>

## Stream-Designer-Symbole {#stream-designer-icons}

In der rechten oberen Ecke des Stream-Designers sehen Sie eine Handvoll Symbole. Hier ist, was sie tun.

<table>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-1.png"></td>
  <td>Vergrößert die Ansicht und erstellt größere Karten</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-2.png"></td>
  <td>Verkleinert die Ansicht und erstellt kleinere Karten</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-3.png"></td>
  <td>Öffnet ein Fenster, in dem Sie Ihren Chat testen können (drücken Sie zum Schließen denselben Knopf)</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-4.png"></td>
  <td>Ermöglicht die Suche nach Karten- oder Inhaltsarten in Ihrem Stream</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-5.png"></td>
  <td>Ordnet alle Karten in Ihrem Stream an</td>
 </tr>
</table>

## Erstellen eines Streams {#create-a-stream}

Sie können Streams für Dialogfelder erstellen oder [Conversation Forms](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}. In diesem Beispiel erstellen wir einen für einen Dialog.

1. Nachdem Sie [Dialogfeld erstellt](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}, klicken Sie auf die **[!UICONTROL Stream-Designer]** Registerkarte.

   ![](assets/stream-designer-6.png)

1. Ziehen Sie die [!UICONTROL Frage] Karte.

   ![](assets/stream-designer-7.png)

1. under [!UICONTROL Chatbot-Antwort], schreiben Sie Ihre Frage, wie Sie möchten.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Sie können das Erlebnis für bekannte Chat-Besucher mit Token personalisieren (z. B.: Hallo `{{lead.leadFirstName:""}}`). Klicken Sie einfach auf das Symbol mit geschweiften Klammern rechts und wählen Sie Ihre Auswahl aus. Fügen Sie einen Standardwert zwischen den Anführungszeichen hinzu, wenn anonyme Besucher etwas Gängiges sehen sollen (z. B.: Hallo `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke ist standardmäßig auf ein gesetzt, wodurch die öffnende Frage neben dem Chat-Symbol angezeigt wird, ohne dass der Besucher darauf klicken muss, um sie zu sehen. Poke ist nur auf der ersten Karte in der Konversation verfügbar.

1. Geben Sie Ihre Benutzerantworten ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**[!UICONTROL Gespeicherte Werte bearbeiten]** ist ein optionaler Schritt für diejenigen, die einen anderen Wert in der Datenbank speichern möchten als das, was Besuchern im Chat-Bot für zugeordnete Attribute in der Fragekarte angezeigt wird (z. B.: Besucher sieht &quot;Suchmaschinenoptimierung&quot;, speichern Sie diesen Wert als &quot;SEO&quot;).

1. Für &quot;Ja&quot; möchten wir einen Termin planen. Ziehen Sie daher unterhalb dieser Option über die Karte Terminplaner .

   ![](assets/stream-designer-10.png)

1. Klicken Sie in der Spalte rechts auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-11.png)

1. Da dies ein Ziel ist, ziehen Sie die [!UICONTROL Ziel] unter dem Terminplaner.

   ![](assets/stream-designer-12.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein vorhandenes aus) und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-13.png)

1. Für &quot;Nein&quot; möchten wir sehen, ob sie der Mailingliste beitreten, also unterhalb dieser Option ziehen Sie über eine andere [!UICONTROL Frage] Karte.

   ![](assets/stream-designer-14.png)

1. Geben Sie Ihre Antwort ein und fügen Sie Antwortoptionen für den Besucher hinzu. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Sie können weitere Antworten hinzufügen, indem Sie **[!UICONTROL Antwort hinzufügen]**.

1. Ziehen Sie unter der Antwort &quot;Ja&quot;über die Karte &quot;Informationserfassung&quot;, damit Sie die E-Mail des Besuchers erfassen können.

   ![](assets/stream-designer-16.png)

1. Klicken Sie auf **[!UICONTROL Typ]** und wählen Sie **[!UICONTROL Email]**.

   ![](assets/stream-designer-17.png)

1. Geben Sie eine Chat-Bot-Nachricht und einen Platzhalter ein. Stellen Sie sicher, dass das Attribut dem entsprechenden Feld in der Marketo Engage zugeordnet ist, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td style="width:30%"><strong>Typ</strong></td>
     <td>Der Informationstyp, den Sie erfassen möchten: Telefon, Text, E-Mail.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Chatbot-Nachricht</strong></td>
     <td>Die Meldung, die der Besucher sieht und ihn auffordert, die Informationen anzugeben.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Platzhalter</strong></td>
     <td>Beispieltext, der dem Besucher dabei hilft, zu sehen, was er eingeben soll.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Antwort einem Attribut zuordnen</strong></td>
     <td>Hiermit können Sie die Antwort des Besuchers mit dem entsprechenden Feld in seinem Personendatensatz in Ihrem Marketo Engage-Abonnement synchronisieren.</td>
    </tr>
   </table>

1. Da die Erfassung ihrer E-Mail ein Ziel ist, ziehen Sie die [!UICONTROL Ziel] Karte unter &quot;Info Capture&quot;angezeigt.

   ![](assets/stream-designer-19.png)

1. Benennen Sie Ihr Ziel (oder wählen Sie ein vorhandenes aus) und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-20.png)

1. Denken Sie daran, eine Antwort hinzuzufügen, wenn Sie &quot;Nein&quot;sagen. Eine Option besteht darin, eine Nachrichten-Karte unten zu ziehen und &quot;Danke trotzdem&quot; zu sagen. Aber in diesem Beispiel stellen wir ihnen stattdessen ein kostenloses PDF-Dokument zur Verfügung.

   ![](assets/stream-designer-21.png)

1. In diesem Beispiel erstellen wir ein neues Dokument. Geben Sie einen Namen ein, geben Sie die URL für die PDF ein, die Sie bereits gehostet haben, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/stream-designer-22.png)

1. Wählen Sie die **[!UICONTROL Vorschau]** Umschalten auf Vorschau des Dialogfelds.

   ![](assets/stream-designer-23.png)

1. Wenn Sie bereit sind, Ihr Dialogfeld zu aktivieren, klicken Sie auf **[!UICONTROL Veröffentlichen]**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Vor dem Klicken [!UICONTROL Veröffentlichen], denken Sie daran, sicherzustellen, dass Sie [Ihre Ziel-URL(s) eingegeben haben](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Erstellen eines Dialogfelds](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Zielgruppenkriterien](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md){target="_blank"}
>* [Adobe PDF Embed API](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}
