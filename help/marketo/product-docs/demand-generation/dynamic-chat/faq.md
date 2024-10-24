---
description: Dynamic Chat FAQ - Marketo Docs - Produktdokumentation
title: Dynamic Chat-FAQs
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: ed833219e5074ae646e07db599e7da50665c453b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Dynamic Chat-FAQs {#dynamic-chat-faq}

Nachstehend finden Sie Antworten auf häufig gestellte Fragen zum Dynamic Chat.

**Ich habe anscheinend keinen Zugriff auf Dynamic Chat. Wie kann ich es bekommen?**

Wenden Sie sich an Ihren Marketo Engage-Administrator und stellen Sie sicher, dass Sie [als Benutzer](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} in der Adobe Admin Console hinzugefügt wurden.

**Kann ich Dynamic Chat irgendwo auf meiner Firmenwebsite installieren oder funktioniert es nur auf Marketo-Einstiegsseiten?**

Das Dynamic Chat JavaScript-Snippet kann auf jeder Website sowie auf Marketo-Landingpages installiert werden.

**Wie lange werden Daten für die Berichterstellung gespeichert?**

90 Tage. Eine vollständige Liste der Einschränkungen/Parameter finden Sie auf der Marketo Engage [Produktbeschreibungsseite](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Unterstützt Dynamic Chat neben Englisch auch andere Sprachen?**

Ja. Dynamic Chat unterstützt die folgenden Sprachen: Französisch, Spanisch, Deutsch, Japanisch, Niederländisch, Italienisch, Brasilianisches Portugiesisch, Koreanisch, Vereinfachtes Chinesisch und Traditionelles Chinesisch. Weitere Informationen finden Sie unter [Ändern der Sprache](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**Unterstützen Sie KI-/NLP-Funktionen?**

Die KI-/NLP-Funktionalität wird nicht unterstützt.

**Wie kann ich anonyme Personen ansprechen?**

In Ihrem Dialogfeld müssen Sie das Attribut _Person Email is Empty_ verwenden.

**Was qualifiziert sich als engagierte Konversation?**

Eine interaktive Konversation tritt auf, sobald ein Besucher in einem Dialogfeld oder einem Konversationsfluss auf den Bot reagiert. Wenn der Besucher den Chat-Bot öffnet, aber nicht auf den Bot reagiert (z. B. Antwort- oder Sendeinformationen), zählt er nicht als Interaktion.

**Was passiert, wenn ich mein monatliches Limit für aktive Konversationen erreicht habe?**

Wenn Sie das monatliche Limit für eingebundene Konversationen erreichen, werden alle veröffentlichten Dialogfelder und Konversationsflüsse nicht mehr ausgelöst, bis Sie Ihr Limit erhöhen oder Ihre Limit zu Beginn des nächsten Monats zurücksetzen.

**Wie erkenne ich, wenn ich mich meinem Limit für die aktive Konversation nähere?**

Wenn Sie 90 % Ihres Limit für interaktive Konversationen erreicht haben, erhalten Dynamic Chat-Administratoren eine E-Mail-Benachrichtigung und allen Benutzern wird eine Bannerbenachrichtigung auf Dynamic Chat angezeigt.

**Wenn ein Besucher mit einem Dialogfeld interagiert und sich anschließend mit einem Live-Agenten verbindet, zählt dies dann als eine oder zwei Interaktionen?**

Für Kunden, die das Paket auswählen, zählt dies als zwei separate Interaktionen - eine für die Dialoginteraktion und eine für die Live-Chat-Interaktion. Bei Kunden mit dem Prime-Paket werden Live-Chatinteraktionen nicht separat gezählt, sodass dies nur als eine Interaktion gezählt wird.

**Wie oft wird die Begrenzung der aktiven Konversation zurückgesetzt?**

Das Limit für die aktive Unterhaltung wird am ersten des Kalendermonats zurückgesetzt.

**Warum kommt der Chatbot nicht zurück, nachdem ich eine Unterhaltung beendet habe?**

Dialogfelder sind so konzipiert, dass sie einem Besucher nur einmal angezeigt werden. Sobald ein Besucher das Ende einer bestimmten Verzweigung in einem Dialogfeld erreicht, wird dieses Dialogfeld als abgeschlossen betrachtet und diesem Besucher nie wieder angezeigt.

**Warum erhalte ich die folgende Nachricht, wenn ich in My Marketo auf die Kachel Dynamic Chat klicke und mich bei Adobe Experience Cloud anmelde? &quot;_Ihr Adobe ID ist anscheinend nicht mit Ihren Adobe Experience Cloud-Lösungskonten verknüpft_&quot;**.

Dies weist höchstwahrscheinlich darauf hin, dass Sie in der Adobe Admin Console nicht als Dynamic Chat-Benutzer hinzugefügt wurden. Wenden Sie sich an einen Systemadministrator für Ihre Adobe-Organisation oder an einen Produktadministrator für Dynamic Chat, um Zugriff auf Dynamic Chat anzufordern.

**Wie greife ich auf das Transkript für eine aktive Unterhaltung zu?**

Dynamic Chat-Transkripte können für jeden bekannten Lead aufgerufen werden, der über die Aktivität &quot;Mit Dynamic Chat-Dialog interagiert&quot;in Marketo Engage mit einem-Dialog interagiert hat und dessen Konvertierungsstatus entweder &quot;Abgeschlossen&quot;oder &quot;Abgelegt&quot;lautet.

**Kann ein Besucher die Konversation neu starten oder zu einer vorherigen Frage zurückkehren, sobald er ein Dialogfeld öffnet?**

Es gibt derzeit keinen systematischen Weg, eine Konversation neu zu starten oder zu einem früheren Punkt zurückzukehren, aber dies ist auf der Dynamic Chat-Roadmap.

**Ist Dynamic Chat in Salesforce integriert?**

Dynamic Chat kann über die Marketo Engage Salesforce-Integration in Salesforce integriert werden.

**Mein Kalender ist mit Dynamic Chat verbunden und ich bin in die Routing-Regeln eingeschlossen. Warum erhalte ich also keine Sitzungen?**

Dies weist höchstwahrscheinlich darauf hin, dass Ihre Kalenderverbindung erneut authentifiziert werden muss. Dies geschieht meistens, wenn Sie Ihr Kennwort für Ihren Kalenderanbieter ändern und Dynamic Chat die Verbindung verliert. Sie können einfach die Seite Agenteneinstellungen unter Dynamic Chat aufrufen und auf &quot;Kalender erneut authentifizieren&quot;klicken.

**Was ist der Unterschied zwischen einem Dialog und einem Konversationsfluss?**

Ein Dialogfeld ist eine Konversation, die Webbesuchern automatisch angezeigt wird, die einen bestimmten Satz von Targeting-Kriterien erfüllen. Ein Konversationsfluss wird nur Besuchern angezeigt, die eine bestimmte Aktion im Internet ausführen, z. B. durch Drücken einer Schaltfläche.

**Gibt es eine Möglichkeit, mit Dynamic Chat Meetings direkt aus einer E-Mail zu buchen?**

Ja! [Erfahren Sie, wie ](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Was genau bedeuten Begriffe wie &quot;Verlobt&quot;oder &quot;Erworbene Personen&quot;?**

Es werden mehrere Begriffe im Dynamic Chat verwendet. Definitionen für viele von ihnen finden Sie in den Hilfeartikeln ihrer jeweiligen Bereiche.

* Analytics-Begriffe wie &quot;Personen, die erworben wurden&quot;[finden Sie hier](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}.
* Definitionen für Smart List-Trigger/Filter [finden Sie hier ](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}.
* Beschreibungen der verschiedenen Stream-Designer-Karten [finden Sie hier](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}.

**Kann ich Dynamic Chat ohne Marketo Engage verwenden?**

Nein. Während Dynamic Chat eine separate Anwendung von Marketo Engage ist, sind die beiden untrennbar miteinander verbunden.
