---
description: Dynamic Chat Übersicht - Marketo Docs - Produktdokumentation
title: Dynamic Chat-Übersicht
feature: Dynamic Chat
source-git-commit: 5e413f280b44691336bd724ddc20936e88d53764
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 2%

---

# Dynamic Chat-Übersicht {#dynamic-chat-overview}

Mit Dynamic Chat können Sie eine benutzerfreundliche Oberfläche nutzen, um sowohl Personen als auch Konten, die Ihre Website besuchen, anzusprechen. Erfassen Sie relevante Inhalte wie Namen, Kontaktinformationen und freien Text. Besucher der Site können auch Meetings mit Ihrem Vertriebsteam buchen. Dynamic Chat-Aktivitäts- und Interaktionsdaten können verwendet werden, um Marketo-Programmen und kanalübergreifenden Aktivitäten von Triggern Mitglieder hinzuzufügen.

>[!TIP]
>
>Besuch [diese Seite](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"} , um Anleitungsvideos zum Dynamic Chat anzuzeigen.

## Integrationen {#integrations}

Eine wichtige Komponente von Dynamic Chat ist die Möglichkeit, nativ mit Ihrem Marketo-Abonnement zu arbeiten. Um die volle Funktionalität dieser Integration nutzen zu können, müssen Sie zunächst die Datensynchronisation starten. Je nach Größe Ihrer Marketo-Datenbank kann es bis zu 24 Stunden dauern, bis Daten für die erste [einmalige Synchronisierung](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"} zu beenden.

Folgendes wird synchronisiert:

* Benutzerfelddaten
* Felddaten des Unternehmens
* Aktivitätsdaten

## Dialoge {#dialogues}

Dialogfelder stellen eine einzige Chatinteraktion dar. Stellen Sie sich dies als Container mit all dem Zeug vor, das Sie benötigen, um einen ansprechenden Chat-Dialog mit Ihren Website-Besuchern zu führen. In jedem Dialogfeld können Sie angeben, auf welchen Seiten das Dialogfeld angezeigt werden soll, wem es angezeigt werden soll und Inhalt und Fluss des Dialogfelds selbst. Darüber hinaus können Sie Metriken finden, um zu sehen, wie gut Ihr Dialogfeld abschneidet. [Weitere Informationen zu Dialogfeldern](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}.

## Konfiguration {#configuration}

Passen Sie auf der Registerkarte Konfiguration das Erscheinungsbild Ihrer verschiedenen Dialogfelder an. Ändern Sie Schriftart, Farben, Antwortzeit und mehr! [Weitere Informationen zur Konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## Kalender {#calendar}

Verbinden Sie Ihren Outlook- oder Gmail-Kalender zur Verwendung bei der Terminplanung im Chatbot. [Weitere Informationen zum Kalender](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Meetings {#meetings}

Hier sehen Sie alle Termine, die von Besuchern der Website über Ihre verschiedenen Dialoge geplant wurden. [Weitere Informationen zu Meetings](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## Routing {#routing}

Hier sehen Sie eine Liste aller Agenten, die ihre Kalender verbunden haben, die Reihenfolge, in der sie den Besuchern der Website angezeigt werden, und erstellen benutzerdefinierte Routing-Regeln. [Weitere Informationen zum Routing](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## Live-Chat {#live-chat}

Bieten Sie Ihren qualifizierten Webbesuchern über [Live-Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## Konversationsfluss {#conversational-flow}

[Konversation gestalten](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"} die von einem Besucher basierend auf einer von Ihnen festgelegten Aktion ausgelöst werden können (z. B. Ausfüllen eines Formulars, Klicken auf einen Link usw.).

## Ändern der Sprache {#changing-the-language}

Führen Sie diese Schritte aus, um Ihre Dynamic Chat-Sprache zu ändern.

>[!IMPORTANT]
>
>Durch das Ändern Ihrer Sprache auf der Profilebene wird die Sprache für _all_ Experience Cloud-Applikationen, nicht nur Dynamic Chat.

1. Klicken Sie in Ihrem Experience Cloud-Konto auf das Einstellungssymbol und wählen Sie **Voreinstellungen**.

   ![](assets/dynamic-chat-overview-1.png)

1. Klicken Sie unter Ihrer E-Mail-Adresse auf die aktuelle Sprache.

   ![](assets/dynamic-chat-overview-2.png)

1. Wählen Sie Ihre neue Sprache aus (die zweite Sprache ist optional) und klicken Sie auf **Speichern**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Es gibt ein paar Dutzend Sprachen zur Auswahl, aber Dynamic Chat unterstützt nur Folgendes: Englisch, Französisch, Deutsch, Japanisch, Spanisch, Italienisch, Portugiesisch (Brasilien), Koreanisch, Chinesisch (vereinfacht) und Chinesisch (traditionell).

Wenn Sie die Sprache aktualisieren, ändert sich alles in der App selbst, mit Ausnahme der Wörter, die Sie persönlich ausgefüllt haben (z. B. Stream-Antworten).

## Dynamic Chat-Datenaufbewahrungsgrenzen {#dynamic-chat-data-retention-limits}

Im Folgenden finden Sie nur einige der Einschränkungen/Parameter innerhalb von Dynamic Chat. Eine vollständige Liste finden Sie im Marketo Engage [Seite &quot;Produktbeschreibung&quot;](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

<table>
  <th>Datentyp</th>
  <th>Bindungszeitraum</th>
 <tr>
  <td>Anonymer Lead ohne Interaktion</td>
  <td>90 Tage</td>
 </tr>
 <tr>
  <td>Zielaktivität</td>
  <td>24 Monate</td>
 </tr>
 <tr>
  <td>Dokumentaktivität</td>
  <td>24 Monate</td>
 </tr>
 <tr>
  <td>Interagiert mit der Dialogfeldaktivität</td>
  <td>90 Tage</td>
 </tr>
 <tr>
  <td>Konferenzbuchungsaktivität</td>
  <td>24 Monate</td>
 </tr>
</table>

## FAQs {#faq}

**Kann ich Dynamic Chat irgendwo auf meiner Firmenwebsite installieren oder funktioniert das nur auf Marketo-Landingpages?**

Das Dynamic Chat JavaScript-Snippet kann auf jeder Website sowie auf Marketo-Landingpages installiert werden.

**Wie lange werden Daten für die Berichterstellung gespeichert?**

90 Tage. Eine vollständige Liste der Beschränkungen/Parameter finden Sie auf der Marketo Engage [Seite &quot;Produktbeschreibung&quot;](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Unterstützt Dynamic Chat neben Englisch auch andere Sprachen?**

Ja. Dynamic Chat unterstützt folgende Sprachen: Französisch, Deutsch, Japanisch, Spanisch, Italienisch, Portugiesisch (Brasilien), Koreanisch, Chinesisch (vereinfacht) und Chinesisch (traditionell). Weitere Informationen finden Sie unter [Abschnitt unten](#changing-the-language).

**Unterstützen Sie KI/NLP-Funktionen?**

Die KI-/NLP-Funktionalität wird nicht unterstützt.

**Wie kann ich anonyme Personen ansprechen?**

In Ihrem Dialogfeld müssen Sie die _Person Email is Empty_ -Attribut.
