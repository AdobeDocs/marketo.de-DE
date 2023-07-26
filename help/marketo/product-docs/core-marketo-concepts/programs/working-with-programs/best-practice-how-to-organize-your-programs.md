---
unique-page-id: 6848705
description: Best Practice - Organisieren Ihrer Programme - Marketo-Dokumente - Produktdokumentation
title: Best Practice - Anleitung zur Organisation Ihrer Programme
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Best Practice: Anleitung zur Organisation Ihrer Programme {#best-practice-how-to-organize-your-programs}

Es gibt viele Möglichkeiten, den Baum in Marketingaktivitäten sowie den Inhalt eines einzelnen Programms zu organisieren. Einige Methoden sind jedoch besser und helfen Benutzern in Ihrer Marketingabteilung.

>[!TIP]
>
>Eines Tages (wenn Sie befördert werden!) Jemand anderes wird versuchen, deine Programme zu verstehen. Eine gute Organisation wird ihnen helfen, schnell produktiv zu sein.

## Ordner {#folders}

In Marketingaktivitäten sollten Sie Ordner verwenden, um Ihre Programme zu organisieren. Die von uns empfohlene Struktur ist im folgenden Beispiel dargestellt:

>[!NOTE]
>
>**Beispiel**
>
>* Aktive Marketingprogramme
>   * E-Mails
>   * Ereignisse
>      * Live-Events/Roadshows
>      * Messen
>      * Webinare
>   * Newsletter
>   * Nurture
>   * Webinhalt
>   * Web-Formulare
>* Lernen
>* Betrieblich
>   * Lebensdauer
>   * Bewertung
>   * Datenverwaltung
>* Sales Insight
>   * Interessante Momente
>   * Verkaufs-E-Mails
>   * Vom Verkauf angeforderte Kampagnen
>* **Archivieren**
>   * Ereignisse archivieren
>      * Archiv 2012
>      * Archiv 2013

Jedes der im Beispiel erwähnten Elemente ist ein Ordner. Beachten Sie, wie sie alle eindeutig benannt sind. Sie können doppelte (einfachere) Namen von Ordnern INSIDE-Programmen haben, aber nicht im Stammverzeichnis des Baums.

>[!TIP]
>
>Der Ordner &quot;Archiv&quot;ist eine spezielle Ordnerart, mit der Elemente aus ausgewählten Listen sowie aus Berichten entfernt werden können. Dies hilft Ihrem System, schneller zu laufen. Lernen [mehr über Ordner](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

Sie können sicherlich weitere Ordner hinzufügen, wenn Sie es für richtig halten. Denken Sie daran, dass zukünftige Generationen von Marketing-Experten in Ihrem Unternehmen mit Ihren Entscheidungen darüber leben, wie Sie Dinge benennen/organisieren.

## Benennungsschemata {#naming-schemes}

Die Benennung ist wichtig, da die Funktionen von Marketo alle eine gemeinsame Sprache für die Kommunikation verwenden. Bei Programmen sollten Sie ihnen etwas Einzigartiges nennen. **Es dürfen keine zwei Programme denselben Namen haben**. Es empfiehlt sich, das folgende Format zu verwenden:

[Abkürzung des Programmtyps] [YYYY]-[MM]-[Optionales DD] [Kurzbeschreibung]

>[!NOTE]
>
>**Beispiel**
>
>Beispiel für Programmnamen:
>
>1. Widget-Einführung ES 2015-09-21
>1. NL Newsletter 2015-06
>1. Webinarthema WBN 2015-12-01 hier

Programmnamen müssen in Ihrem Abonnement eindeutig sein, auch in verschiedenen [Arbeitsbereiche](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  Für lokale Assets innerhalb von Programmen gilt folgende Regel: **einfachen Namen beibehalten**. Benennen Sie einfach eine Einladung mit &quot;Einladung&quot;, anstatt mit &quot;Einladung im Webinar vom Juni 2015&quot;. Da sich diese in einem Programm befinden, ist das übergeordnete Programm automatisch Teil des Namens, wenn es an einer anderen Stelle ausgewählt wird. Anders ausgedrückt: Lokale Assets müssen nur innerhalb des Programms eindeutig sein. Sie können Hunderte von Assets mit dem Namen &quot;Einladen&quot;haben, die jeweils in einem anderen Programm gespeichert sind, sodass Sie sich nicht daran stören.

## Token {#tokens}

Token verwenden Ordner und Programme als Vehikel, um Variablen festzulegen, die von Landingpages, E-Mails und anderen Assets verwendet werden.

Die oben erwähnte Organisation ermöglicht es Ihnen, Token in den Ordner &quot;Event&quot;zu verschieben, damit sie in alle Ereignisse kaskadiert werden.

>[!NOTE]
>
>**Beispiel**
>
>**Ihre Firmenadresse**. Verwenden Sie ein Token, anstatt es jedes Mal zu schreiben. Auf diese Weise können Sie es an einem Ort aktualisieren, ohne dass Sie viele Entwürfe erstellen müssen. Überschreiben Sie dann das Token nach Bedarf in einem Ordner der unteren Ebene.

## Ereignisse {#events}

Ein Ereignis enthält in der Regel viele bewegte Teile, darunter Einladungen, Landingpages, Formulare, Social-Widgets und Smart-Kampagnen. Die Best Practice, sie zur einfachen Verwendung zu organisieren, ist die Phase des Ereignisses. Im Folgenden finden Sie ein Beispiel dafür, wie Ihr Ordnerbaum nach einem Ereignis suchen sollte.

![](assets/capture.png)

## Engagementprogramme {#engagement-programs}

Lernen [Interaktionsprogramme](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). Die beste Möglichkeit, Ihr Interaktionsprogramm zu organisieren, besteht in Ordnern. Erstellen Sie einen Ordner für jeden Stream und legen Sie dann die E-Mails oder Programme in diesen Ordner. Fügen Sie in jedem Stream einen Archivordner ein, wenn der Inhalt veraltet ist und Sie ihn entfernen möchten.

## Operationelle Programme {#operational-programs}

Diese werden für Datenbereinigungszwecke verwendet. Verfügen über Ordner für die Daten, zu denen die Programme ausgeführt wurden, und archivieren Sie dann die Ordner. Wenn Sie das Programm in die Praxis umsetzen, entziehen Sie es der Berichterstattung, was für diese Art von Aktivität von Vorteil ist.

## Verschachteln von E-Mail-Programmen {#nesting-email-programs}

E-Mail-Programme sind Ihr Tool für das Briefpost-Strahling. Sie können sie in Veranstaltungen oder andere Programme für Promotions, Einladungen und Erinnerungen einfügen. Sie enthalten ein cooles Dashboard und andere A/B-Test-Funktionen. Darüber hinaus können sie einfach in der Programmplanungsansicht bearbeitet werden.

Sie können auch ein E-Mail-Programm als eigenständiges Programm erstellen. E-Mail-Programme sind in anderen E-Mail-Programmen nicht zulässig. Das wäre verrückt!

## Wird geklont {#cloning}

Eine der coolsten Funktionen in Marketo ist die Möglichkeit, Programme zu klonen. Dies bedeutet, dass Sie eine Programmvorlage einrichten können, die alle gewünschten Smart-Kampagnen und E-Mails enthält. Richten Sie es im Voraus ein und klonen Sie es dann für Ihre nächste Marketing-Initiative.

>[!TIP]
>
>Beachten Sie die Ereignisvorlagen im Beispiel oben. Legen Sie Ihre verschiedenen Arten von Ereignissen dort hin, um das Klonen zu erleichtern.

Manche Personen haben sogar den Großteil des Textes in E-Mails und Landingpages in Token abstrahiert. Auf diese Weise können Sie die Token klonen und dann bearbeiten. Gehen Sie schließlich zur Programmplanungsansicht und passen Sie die Daten an und Sie sind fertig. Voila!

## Zusammenfassung {#summary}

Wie Sie sehen können, gibt es in Marketo eine Menge Macht. Wir haben die Grundlagen hier behandelt, aber einige [zusätzliche Dienste von Marketo-Experten](https://www.marketo.com/services/) , um sich für den Erfolg zu rüsten und sich selbst einzurichten.
