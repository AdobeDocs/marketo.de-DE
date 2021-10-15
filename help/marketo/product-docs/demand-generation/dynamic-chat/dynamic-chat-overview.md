---
description: Übersicht über dynamischen Chat - Marketo-Dokumente - Produktdokumentation
title: Übersicht über dynamischen Chat
hide: true
hidefromtoc: true
source-git-commit: 1434d2a1cbf5575cea60ccc0c655313003b1452c
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Übersicht über dynamischen Chat {#dynamic-chat-overview}

Mit dem dynamischen Chat können Sie eine benutzerfreundliche Oberfläche nutzen, um sowohl Personen als auch Konten, die Ihre Website besuchen, als Ziel anzusehen. Erfassen Sie relevante Inhalte wie Namen, Kontaktinformationen und freien Text. Besucher der Site können auch Meetings mit Ihrem Vertriebsteam buchen. Die Aktivitäts- und Interaktionsdaten des dynamischen Cats können verwendet werden, um Marketo-Programmen und kanalübergreifenden Aktivitäten von Triggern Mitglieder hinzuzufügen.

>[!NOTE]
>
>Der dynamische Chat wird derzeit schrittweise eingeführt und ist derzeit in begrenztem Umfang verfügbar. Diese Seite wird mit den allgemeinen Verfügbarkeitsdetails (GA) aktualisiert, sobald sie verfügbar werden.

## Integrationen {#integrations}

Eine wichtige Komponente des dynamischen Chat ist die Möglichkeit, nativ mit Ihrem Marketo-Abonnement zu arbeiten. Um die volle Funktionalität dieser Integration nutzen zu können, müssen Sie zunächst die Datensynchronisation starten. Je nach Größe Ihrer Marketo-Datenbank kann es bis zu 24 Stunden dauern, bis die Daten zum ersten Mal ([einmalige Synchronisation](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md)) synchronisiert sind. Die durchschnittliche Synchronisierungszeit beträgt weniger als zwei Stunden.

Folgendes wird synchronisiert:

* Benutzerfelddaten
* Felddaten des Unternehmens
* Aktivitätsdaten

## Dialogfelder {#dialogues}

Dialogfelder stellen eine einzige Chatinteraktion dar. Stellen Sie sich dies als Container mit all dem Zeug vor, das Sie benötigen, um einen ansprechenden Chat-Dialog mit Ihren Website-Besuchern zu führen. In jedem Dialogfeld können Sie angeben, auf welchen Seiten das Dialogfeld angezeigt werden soll, wem es angezeigt werden soll und Inhalt und Fluss des Dialogfelds selbst. Darüber hinaus können Sie Metriken finden, um zu sehen, wie gut Ihr Dialogfeld abschneidet. [Weitere Informationen zu Dialogfeldern](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Konfiguration {#configuration}

Passen Sie auf der Registerkarte Konfiguration das Erscheinungsbild Ihrer verschiedenen Dialogfelder an. Ändern Sie Schriftart, Farben, Antwortzeit und mehr! [Weitere Informationen zur Konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Kalender {#calendar}

Verbinden Sie auf der Registerkarte Kalender Ihren Kalender (Outlook oder Gmail) für die Verwendung bei der Terminplanung im Chat. Sobald der Kalender eines Benutzers mit dem dynamischen Chat verbunden ist, wird dieser Benutzer zur Warteschlange hinzugefügt und sein Kalender steht Website-Besuchern zur Verfügung, um Termine zu planen.

Sie können auch den Text der Einladung anpassen, die dem Besucher gesendet wird, wenn er einen Termin im Kalender des Benutzers einplant.

## Sitzungen {#meetings}

Hier sehen Sie alle Termine, die von Besuchern der Website über Ihre verschiedenen Dialoge geplant wurden. Hier finden Sie die E-Mail-Adresse der Person, die den Termin gebucht hat, den Agenten, mit dem sie den Termin gebucht haben, wann der Termin geplant ist und ob das Treffen stattgefunden hat oder nicht.

## Routing {#routing}

Hier sehen Sie eine Liste aller Agenten, die ihre Kalender verbunden haben, sowie die Reihenfolge, in der sie den Besuchern der Website angezeigt werden. Meetings gehen um Robin-Stil. Wenn Sie also fünf Agenten und Agenten drei haben, die das letzte Meeting hatten, werden Agent vier das nächste bekommen, gefolgt von Agent fünf, dann zurück zum Agenten eins.

## FAQs {#faq}

**Ermöglicht der dynamische Chat einen Live-Chat?**

Nein, es werden nur vordefinierte Antworten verwendet.

**Wie kann ich anonyme Personen ansprechen?**

In Ihrem Dialogfeld müssten Sie das Attribut _Person Email is Empty_ verwenden.

**Unterstützen Sie KI/NLP-Funktionen?**

Die KI-/NLP-Funktionalität wird nicht unterstützt.

**Wie lange werden Daten für Berichte gespeichert?**

90 Tage.

**Bietet Dynamic Chat neben Englisch auch andere Sprachen?**

Zum jetzigen Zeitpunkt nicht.
