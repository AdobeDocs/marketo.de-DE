---
description: Häufig gestellte Fragen zu Dynamic Chat - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Dynamic Chat
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Dynamic Chat {#dynamic-chat-faq}

Im Folgenden finden Sie Antworten auf einige häufig gestellte Fragen zu Dynamic Chat.

**Ich habe anscheinend keinen Zugang zu Dynamic Chat. Wie bekomme ich es?**

Wenden Sie sich an Ihren Marketo Engage-Administrator und stellen Sie sicher, dass er [Sie als Benutzer hinzugefügt](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} in der Adobe Admin Console hat.

**Kann ich Dynamic Chat an einer beliebigen Stelle auf meiner Unternehmens-Website installieren oder funktioniert es nur auf Marketo-Landingpages?**

Das Dynamic Chat JavaScript-Snippet kann auf jeder Website sowie auf Landingpages von Marketo installiert werden.

**Wie lange werden Daten für das Reporting gespeichert?**

90 Tage. Eine vollständige Liste der Grenzwerte/Parameter finden Sie auf der Marketo Engage-[Produktbeschreibungsseite](https://helpx.adobe.com/de/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Unterstützt Dynamic Chat neben Englisch auch andere Sprachen?**

Ja. Dynamic Chat unterstützt die folgenden Sprachen: Französisch, Spanisch, Deutsch, Japanisch, Niederländisch, Italienisch, Portugiesisch (Brasilien), Koreanisch, Chinesisch (vereinfacht) und Chinesisch (traditionell). Weitere Informationen finden Sie unter [Ändern der &#x200B;](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**Unterstützen Sie KI-/NLP-Funktionen?**

KI-/NLP-Funktionen werden nicht unterstützt.

**Wie kann ich anonyme Personen ansprechen?**

In Ihrem Dialogfeld müssten Sie das Attribut _Person E-Mail ist leer_ verwenden.

**Was gilt als engagiertes Gespräch?**

Eine interaktive Konversation tritt auf, sobald ein Besucher in einem Dialog- oder Konversationsfluss auf den Bot antwortet. Wenn der Besucher den Chat-Bot öffnet, aber nicht auf den Bot reagiert (z. B. eine Antwort auswählen oder Informationen übermitteln), wird dies nicht als Interaktion gezählt.

**Was passiert, wenn ich mein monatliches Limit für interaktive Gespräche erreicht habe?**

Wenn Sie das monatliche Limit für interaktive Konversationen erreicht haben, werden alle veröffentlichten Dialogfelder und Konversationsflüsse nicht mehr ausgelöst, bis Sie Ihr Limit erhöhen oder Ihr Limit zu Beginn des nächsten Monats zurückgesetzt wird.

**Woher weiß ich, wann ich mich meinem Limit für interaktive Gespräche nähere?**

Wenn Sie 90 % des Limits für interaktive Konversationen erreicht haben, erhalten Dynamic Chat-Admins eine E-Mail-Benachrichtigung und alle Benutzenden sehen eine Bannerbenachrichtigung in Dynamic Chat.

**Wenn ein Besucher mit einem Dialogfeld interagiert und dann anschließend eine Verbindung zu einem Live-Agenten herstellt, zählt dies dann als eine oder zwei Interaktionen?**

Für Kunden mit dem Select-Paket wird dies als zwei separate Interaktionen gezählt - eines für die Interaktion mit dem Dialog und eines für die Interaktion mit dem Live-Chat. Für Kunden mit dem Prime-Package werden Live-Chat-Interaktionen nicht separat gezählt, sodass dies nur als eine Interaktion zählt.

**Wie oft wird das Interaktionslimit zurückgesetzt?**

Das Limit für interaktive Konversationen wird am ersten Tag jedes Kalendermonats zurückgesetzt.

**Warum kommt der Chatbot nicht zurück, nachdem ich ein Gespräch beendet habe?**

Dialogfelder sind so konzipiert, dass sie einem Besucher nur einmal angezeigt werden. Sobald also ein Besucher das Ende einer bestimmten Verzweigung in einem Dialogfeld erreicht, wird dieses Dialogfeld als abgeschlossen betrachtet und diesem Besucher nie wieder angezeigt.

**Warum erhalte ich die folgende Meldung, wenn ich in Meine Marketo auf die Kachel Dynamic Chat klicke und mich bei Adobe Experience Cloud anmelde? &quot;_Es scheint, dass Ihre Adobe ID nicht mit Ihren Adobe Experience Cloud-Lösungskonten verknüpft ist_.“**

Dies weist höchstwahrscheinlich darauf hin, dass Sie nicht als Dynamic Chat-Benutzende in der Adobe Admin Console hinzugefügt wurden. Wenden Sie sich entweder an einen Systemadministrator für Ihre Adobe-Organisation oder an einen Produktadministrator für Dynamic Chat, um Zugriff auf Dynamic Chat zu erhalten.

**Wie greife ich auf das Transkript für ein interaktives Gespräch zu?**

Auf Dynamic Chat-Transkripte kann für jeden bekannten Lead zugegriffen werden, der über die Aktivität „Mit Dialog interagiert“ in Marketo Engage mit einem Dynamic Chat-Dialogfeld interagiert hat und dessen Konversationsstatus entweder „Abgeschlossen“ oder „Abgebrochen“ lautet.

**Wenn ein Besucher in ein Dialogfeld eintritt, kann er das Gespräch neu starten oder zu einer vorherigen Frage zurückkehren?**

Es gibt derzeit keine systematische Möglichkeit, ein Gespräch neu zu beginnen oder zu einem vorherigen Punkt zurückzukehren, aber dies steht auf dem Dynamic Chat-Fahrplan.

**Ist Dynamic Chat mit Salesforce integriert?**

Dynamic Chat lässt sich über die Marketo Engage Salesforce-Integration mit Salesforce integrieren.

**Mein Kalender ist in Dynamic Chat verbunden und ich bin in den Routing-Regeln enthalten, warum erhalte ich also keine Meetings?**

Dies weist höchstwahrscheinlich darauf hin, dass Ihre Kalenderverbindung erneut authentifiziert werden muss. Dies tritt am häufigsten auf, wenn Sie das Kennwort für Ihren Kalenderanbieter ändern und Dynamic Chat die Verbindung verliert. Sie können einfach zur Seite mit den Agenteneinstellungen in Dynamic Chat gehen und auf „Kalender erneut authentifizieren“ klicken.

**Was ist der Unterschied zwischen einem Dialog und einem Konversationsfluss?**

Ein Dialogfeld ist eine Konversation, die Web-Besuchern, die einen definierten Satz von Zielgruppenbestimmungskriterien erfüllen, automatisch angezeigt wird. Ein Konversationsfluss wird nur Besuchern angezeigt, die eine bestimmte Aktion im Web durchführen, z. B. eine Schaltfläche drücken.

**Gibt es eine Möglichkeit, Dynamic Chat zu verwenden, um Meetings direkt über eine E-Mail zu buchen?**

Ja! [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Was genau bedeuten Begriffe wie „Interagiert“ oder „Erworbene Personen“?**

In Dynamic Chat werden mehrere Begriffe verwendet. Definitionen für viele von ihnen finden Sie in den Hilfeartikeln der jeweiligen Bereiche.

* Analytics-Begriffe wie „Personen erworben[&#x200B; (finden Sie hier](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}.
* Trigger-/Filterdefinitionen für Smart-Listen [finden Sie hier](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}.
* Beschreibungen der verschiedenen Stream Designer-Karten [finden Sie hier](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}.

**Kann ich Dynamic Chat ohne Marketo Engage verwenden?**

Nein. Dynamic Chat ist zwar ein separates Programm von Marketo Engage, aber die beiden sind untrennbar miteinander verbunden.
