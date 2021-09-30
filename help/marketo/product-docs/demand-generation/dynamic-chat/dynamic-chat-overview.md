---
description: Übersicht über dynamischen Chat - Marketo-Dokumente - Produktdokumentation
title: Übersicht über dynamischen Chat
hide: true
hidefromtoc: true
source-git-commit: b6f0b24ef1e9cece06f44ae11d432291b8ac0425
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Übersicht über dynamischen Chat {#dynamic-chat-overview}

Mit dem dynamischen Chat können Sie eine benutzerfreundliche Oberfläche nutzen, um beide Leads (PEOPLE?) und Konten auf ihrer (BESUCHEN SIE IHRE?) Website. Erfassen Sie relevante Inhalte wie ihren Namen, Kontaktinformationen und freien Text. Besucher der Site können auch Meetings mit Ihrem Vertriebsteam buchen. Die Aktivitäts- und Interaktionsdaten des dynamischen Cats können verwendet werden, um Marketo-Programmen und kanalübergreifenden Aktivitäten von Triggern Mitglieder hinzuzufügen.

>[!NOTE]
>
>Der dynamische Chat wird derzeit schrittweise eingeführt und ist derzeit in begrenztem Umfang verfügbar. Diese Seite wird mit den allgemeinen Verfügbarkeitsdetails (GA) aktualisiert, sobald sie verfügbar werden.

## Integrationen {#integrations}

Eine wichtige Komponente des dynamischen Chat ist die Möglichkeit, nativ mit Ihrem Marketo-Abonnement zu arbeiten. Um die volle Funktionalität dieser Integration nutzen zu können, müssen Sie zunächst die Datensynchronisation starten. Je nach Größe Ihrer Marketo-Datenbank kann es bis zu 24 Stunden dauern, bis die Daten zum ersten Mal ([einmalige Synchronisation](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md)) synchronisiert sind. Die durchschnittliche Synchronisierungszeit beträgt weniger als zwei Stunden.

Folgendes wird synchronisiert:

* Lead-Felddaten
* Felddaten des Unternehmens
* Aktivitätsdaten

## Dialogfelder {#dialogues}

Dialogfelder stellen eine einzige Chatinteraktion dar. Stellen Sie sich dies als Container mit all dem Zeug vor, das Sie benötigen, um einen ansprechenden Chat-Dialog mit Ihren Website-Besuchern zu führen. In jedem Dialogfeld können Sie angeben, auf welchen Seiten das Dialogfeld angezeigt werden soll, wem es angezeigt werden soll und Inhalt und Fluss des Dialogfelds selbst. Darüber hinaus können Sie Metriken finden, um zu sehen, wie gut Ihr Dialogfeld abschneidet. [Weitere Informationen zu Dialogfeldern](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Konfiguration {#configuration}

Passen Sie auf der Registerkarte Konfiguration das Erscheinungsbild Ihrer verschiedenen Dialogfelder an. Ändern Sie Schriftart, Farben, Antwortzeit und mehr! [Weitere Informationen zur Konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Kalender {#calendar}

Verbinden Sie auf der Registerkarte Kalender Ihren Kalender (Outlook oder Gmail) für die Verwendung bei der Terminplanung im Chat. Sobald der Kalender eines Benutzers mit dem dynamischen Chat verbunden ist, wird dieser Benutzer zur Warteschlange hinzugefügt und sein Kalender steht Website-Besuchern zur Verfügung, um Termine zu planen.

Sie können auch den Text der Einladungs-E-MAIL anpassen? , der dem Besucher bei der Planung eines Termins im Kalender des Benutzers gesendet wird.

## Sitzungen {#meetings}

Hier sehen Sie alle Termine, die von Besuchern der Website über Ihre verschiedenen Dialoge geplant wurden. Hier finden Sie die E-Mail-Adresse des Leads, der den Termin gebucht hat, mit welchem Agenten er den Termin gebucht hat, wann der Termin geplant ist und ob das Treffen stattgefunden hat oder nicht.

## Routing {#routing}

Hier können Sie eine Liste aller Agenten sehen, die ihre Kalender verbunden haben, sowie die Reihenfolge, in der sie den Besuchern der Website präsentiert werden Meetings gehen im Robin-Stil. Wenn Sie also fünf Agenten haben und drei Agenten das letzte Meeting hatten, erhalten Agent vier das nächste, gefolgt von fünf und dann zurück zum Agenten.

## FAQs {#faq}

**Ermöglicht der dynamische Chat einen Live-Chat?**

Nein, es werden nur vordefinierte Antworten verwendet.

**Wie kann ich anonyme Leads ansprechen?**

In Ihrem Dialogfeld müssten Sie das Attribut _Lead-E-Mail ist leer_ verwenden.

**Unterstützen Sie KI/NLP-Funktionen?**

Die KI-/NLP-Funktionalität wird nicht unterstützt.

**Wie lange werden Daten für Berichte gespeichert?**

90 Tage.

**Bietet Dynamic Chat neben Englisch auch andere Sprachen?**

Zum jetzigen Zeitpunkt nicht.
