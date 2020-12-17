---
unique-page-id: 2359545
description: Definieren Sie die Kriterien für den Gewinner des A/B-Tests - Marketing-Dokumente - Produktdokumentation
title: Definieren der Kriterien für den A/B-Test-Gewinner
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Definieren Sie die Kriterien für den Gewinner des A/B-Tests {#define-the-a-b-test-winner-criteria}

Wenn Sie [einen A/B-Test](add-an-a-b-test.md) zu Ihrem E-Mail-Programm hinzufügen, müssen Sie einen Testtyp auswählen: [Planen Sie den A/B-Test](schedule-the-a-b-test.md) und legen Sie dann die Gewinnerkriterien fest. Hier ist, wie man entscheidet, welche E-Mail gewinnt.

>[!PREREQUISITES]
>
>* [hinzufügen eines A/B-Tests](add-an-a-b-test.md)

>



## Gewinnerkriterien {#winner-criteria}

1. Zuerst werden die Standardoptionen **Gewinnerkriterien** aufgelistet.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Öffnen** | Ein geöffnetes Fenster registriert sich, wenn Bilder in eine E-Mail heruntergeladen werden. Auch wenn Sie kein Bild einschließen, fügt Marketo standardmäßig ein einzelnes Verfolgungs-Pixel in alle HTML-E-Mails ein. |
   |---|---|
   | **Klicks** | Standardmäßig sind Links in E-Mails mit einer Verfolgung versehen, die es Ihnen ermöglicht, zu sehen, wer auf welchen Link geklickt hat, wie viele Links insgesamt angeklickt wurden usw. |
   | **Zum Öffnen % klicken** | Prozentsatz der E-Mails, die geöffnet wurden und auf die ein Link in der E-Mail geklickt wurde. Damit werden Relevanz und Kontext einer E-Mail gemessen, indem die Anzahl der individuellen Klicks geteilt durch die Anzahl der individuellen Eröffnungen und dann durch 100 multipliziert werden, um den Prozentsatz anzuzeigen. |
   | **Interaktionsbewertung** | Das [Interaktionsergebnis](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score) hilft Ihnen bei der Bestimmung der Effektivität Ihres Inhalts. |

   >[!TIP]
   >
   >Wenn Sie Interaktionsbewertung auswählen, muss der Test mindestens 24 Stunden lang ausgeführt werden. Erfahren Sie mehr über [das Verstehen des Interaktionswerts](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

   Sie können Ihre Kriterien auch anpassen, indem Sie Benutzerspezifische Konversion auswählen und auf Bearbeiten klicken.
   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Mit der benutzerdefinierten Konversion können Sie jedes beliebige Ereignis als Konversion auswählen, indem Sie Auslöser und Filter verwenden.

   Daraufhin wird ein Fenster geöffnet. Suchen Sie den Auslöser Ihrer Wahl und ziehen Sie ihn auf die Arbeitsfläche.
   ![](assets/image2014-9-12-15-3a52-3a18.png)

   >[!NOTE]
   >
   >**Tieftauchen**
   >
   >
   >Erfahren Sie mehr über [intelligente Listen und statische Listen](http://docs.marketo.com/display/docs/smart+lists+and+static+lists).

   Definieren Sie den Auslöser.
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo erlaubt nur Auslöser für Personen, die die E-Mail von diesem E-Mail-Programm erhalten haben. Es ist nicht erforderlich, den Filter &quot;Wurde gesendet&quot; hinzuzufügen.

   Klicken Sie auf Schließen.
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Großartig! Jetzt ist es an der Zeit zu entscheiden, wie der Gewinner bestimmt wird.

## Gewinner bekannt geben {#declare-winner}

1. Wählen Sie eine der beiden verfügbaren Optionen aus.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Wenn Sie einen **Date/Time** A/B-Test durchführen, können Sie nur **Manuell** auswählen.

   Sobald der A/B-Test beendet ist, kann Marketo die erfolgreichste E-Mail automatisch zur geplanten Zeit senden oder Sie können die Ergebnisse überprüfen und entscheiden, welche E-Mail nach Ablauf gesendet wird.

1. Automatisch ist fantastisch und die Standardoption. Klicken Sie einfach auf **Weiter**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Wenn Sie **Manuell** wählen, wird der Test gesendet und es wird gewartet, bis Sie einen Gewinner angeben. Sie erhalten einen Bericht über die Ergebnisse.

   [Plan des A/B-Tests](schedule-the-a-b-test.md)

Perfekt! Jetzt lasst uns .