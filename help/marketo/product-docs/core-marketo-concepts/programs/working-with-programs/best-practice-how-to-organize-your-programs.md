---
unique-page-id: 6848705
description: Best Practice - Organisieren von Programmen - Marketo-Dokumente - Produktdokumentation
title: 'Best Practice : Organisieren von Programmen'
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 5%

---

# Best Practice: Organisieren von Programmen {#best-practice-how-to-organize-your-programs}

Es gibt viele Möglichkeiten, den Baum in Marketing-Aktivitäten sowie den Inhalt eines einzelnen Programms zu organisieren. Einige Wege sind jedoch besser und helfen den Leuten in Ihrer Marketing-Abteilung.

>[!TIP]
>
>Eines Tages (wenn Sie befördert werden!) wird jemand anderes versuchen, Ihre Programme zu verstehen. Eine gute Organisation wird ihnen helfen, schnell produktiv zu sein.

## Ordner {#folders}

In Marketing-Aktivitäten sollten Sie Ihre Programme mit Ordnern organisieren. Die von uns empfohlene Struktur ist im folgenden Beispiel:

>[!NOTE]
>
>**Beispiel**
>
>* Aktive Marketingprogramme
>   * E-Mails
>   * Ereignisse
>     * Live-Events/Roadshows
>     * Messen
>     * Webinare
>   * Newsletter
>   * Nurture-Kampagne
>   * Web-Inhalt
>   * Web-Formulare
>* Lernvorgang läuft
>* Betrieblich
>   * Lebenszyklus
>   * Bewertung
>   * Daten-Management
>* Sales Insight
>   * Interessante Momente
>   * Verkaufs-E-Mails
>   * Vom Verkauf angeforderte Kampagnen
>* **Archivieren**
>   * Ereignisse archivieren
>     * Archiv 2012
>     * Archiv 2013

Jede der im Beispiel genannten ist ein Ordner. Beachten Sie, dass alle eindeutig benannt sind. Sie können doppelte (einfachere) Namen von Ordnern INNERHALB von Programmen haben, aber nicht am Stamm der Baumstruktur.

>[!TIP]
>
>Der Ordner „Archiv“ ist eine spezielle Art von Ordner, der dazu dient, Elemente aus ausgewählten Listen zu entfernen und Berichte zu erstellen. Dadurch kann Ihr System schneller ausgeführt werden. Weitere [ zu Ordnern](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md){target="_blank"}.

Sie können sicherlich weitere Ordner hinzufügen, wie Sie es für richtig halten. Denken Sie daran, dass zukünftige Generationen von Marketern in Ihrem Unternehmen mit Ihren Entscheidungen über die Benennung/Organisation von Dingen leben werden.

## Benennungsschemata {#naming-schemes}

Die Benennung ist von entscheidender Bedeutung, da die Funktionen von Marketo alle eine gemeinsame Sprache für die Kommunikation verwenden. Für Programme sollten Sie ihnen etwas Einzigartiges nennen. **Zwei Programme dürfen nicht denselben Namen haben**. Es empfiehlt sich, das folgende Format zu verwenden:

[Abkürzung für Programmtyp] [JJJJ]-[MM]-[] Optional TT[Kurzbeschreibung]

>[!NOTE]
>
>**Beispiel**
>
>Beispiel für Programmnamen:
>
>1. ES 2015-09-21 Widget Intro
>1. NL 2015-06 Newsletter
>1. WBN 2015-12-01 Webinar Thema hier

Programmnamen müssen in Ihrem Abonnement eindeutig sein, auch in verschiedenen [Arbeitsbereichen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md){target="_blank"}.  Für lokale Assets innerhalb von Programmen lautet die Regel **Halten des Namens einfach**. Geben Sie einfach eine Einladung als „Einladung“ und nicht als „Einladung zum Juni-Webinar 2015“ ein. Da diese sich in einem Programm befinden, ist das übergeordnete Programm automatisch Teil des Namens, wenn Sie es an einer anderen Stelle auswählen. Mit anderen Worten: Lokale Assets müssen nur innerhalb des Programms eindeutig sein. Sie können Hunderte von Assets mit dem Namen „Einladen“ in jeweils einem anderen Programm haben, und es wird Sie nicht durcheinander bringen.

## Token {#tokens}

Token verwenden Ordner und Programme als Mittel zum Festlegen von Variablen, die von Landingpages, E-Mails und anderen Assets verwendet werden können.

Die oben genannte Organisation ermöglicht es Ihnen, Token im Ereignisordner abzulegen, sodass er in alle Ereignisse übergeht.

>[!NOTE]
>
>**Beispiel**
>
>**Ihre Unternehmensadresse**. Benutze ein Token, anstatt es jedes Mal zu schreiben. Auf diese Weise können Sie sie an einer Stelle aktualisieren, ohne viele Entwürfe erstellen zu müssen. Überschreiben Sie dann das Token nach Bedarf in einem Ordner auf niedrigerer Ebene.

## Ereignisse {#events}

Ein Event hat in der Regel viele bewegte Teile, darunter Einladungen, Landingpages, Formulare, Social-Widgets und intelligente Kampagnen. Die Best Practice für ihre Organisation zur Benutzerfreundlichkeit ist die Phase der Veranstaltung. Im Folgenden finden Sie ein Beispiel dafür, wie die Ordnerstruktur nach einem Ereignis aussehen sollte.

![](assets/capture.png)

## Interaktionsprogramme {#engagement-programs}

Erfahren [ alles über Interaktionsprogramme](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md){target="_blank"}. Die beste Möglichkeit, Ihr Interaktionsprogramm zu organisieren, besteht in Ordnern. Erstellen Sie für jeden Stream einen Ordner und legen Sie dann die E-Mails oder Programme in diesem Ordner ab. Fügen Sie in jeden Stream einen Archivordner ein, wenn der Inhalt veraltet ist und Sie ihn entfernen möchten.

## Operationelle Programme {#operational-programs}

Diese werden zur Datenbereinigung verwendet. Legen Sie Ordner für die Daten bereit, an denen die Programme ausgeführt wurden, und archivieren Sie dann die Ordner. Indem Sie das Programm operationell machen, lassen Sie es bei der Berichterstattung weg, was für diese Art von Aktivität gut ist.

## Verschachteln von E-Mail-Programmen {#nesting-email-programs}

E-Mail-Programme sind als Tool für Mail-Blasting konzipiert. Sie können sie in Veranstaltungen oder andere Programme für Werbeaktionen, Einladungen und Erinnerungen einfügen. Sie verfügen über ein cooles Dashboard und andere A/B-Testfunktionen. Darüber hinaus können sie in der Programmplanansicht einfach bearbeitet werden.

Sie können auch ein E-Mail-Programm als eigenständiges Programm erstellen. E-Mail-Programme sind in anderen E-Mail-Programmen nicht zulässig. Das wäre verrückt!

## Wird geklont {#cloning}

Eine der coolsten Funktionen in Marketo ist die Möglichkeit, Programme zu klonen. Dies bedeutet, dass Sie eine Programm-„Vorlage“ einrichten können, die alle gewünschten intelligenten Kampagnen und E-Mails enthält. Richten Sie ihn im Voraus ein und klonen Sie ihn dann für Ihre nächste Marketing-Initiative.

>[!TIP]
>
>Beachten Sie die Ereignisvorlagen im Beispiel oben. Stellen Sie Ihre verschiedenen Arten von Ereignissen bereit, um das Klonen zu erleichtern.

Einige Personen abstrahieren sogar den Großteil des Textes in E-Mails und Landingpages in Token. Auf diese Weise können Sie die Token klonen und dann bearbeiten. Rufen Sie abschließend die Ansicht Programmplan auf, passen Sie die Daten an und Sie sind fertig. Voila!

## Zusammenfassung {#summary}

Wie Sie sehen können, gibt es viel Macht in Marketo. Wir haben hier die Grundlagen behandelt, erwägen jedoch zusätzliche Services von [Marketo Engage-](https://business.adobe.com/products/marketo/services-support.html){target="_blank"}, um eine Feinabstimmung vorzunehmen und sich für den Erfolg einzurichten.
