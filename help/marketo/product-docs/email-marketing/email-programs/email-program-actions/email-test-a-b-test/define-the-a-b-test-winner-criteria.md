---
unique-page-id: 2359545
description: Definieren der A/B-Test-Gewinnerkriterien - Marketo Docs - Produktdokumentation
title: Definieren der A/B-Test-Gewinnerkriterien
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 3%

---

# Definieren der A/B-Test-Gewinnerkriterien {#define-the-a-b-test-winner-criteria}

Wenn Sie [A/B-Test hinzufügen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}, müssen Sie einen Testtyp auswählen, den A/B-Test planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"} und dann die Gewinnerkriterien definieren. [ Hier erfahren Sie, wie Sie entscheiden, welche E-Mail gewinnt.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Gewinnerkriterien {#winner-criteria}

1. Die standardmäßigen Optionen für **Gewinnerkriterien** werden zuerst aufgelistet.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Geöffnet</b></td>
   <td>Ein offenes Feld registriert sich, wenn Bilder in eine E-Mail heruntergeladen werden. Auch wenn Sie kein Bild angeben, fügt Marketo standardmäßig ein einzelnes Tracking-Pixel in alle HTML-E-Mails ein.</td>
   </tr>
   <tr>
   <td><b>Klicks</b></td>
   <td>Standardmäßig sind Links in E-Mails mit eingebettetem Tracking versehen, sodass Sie sehen können, wer auf welchen Link geklickt hat, wie viele Links insgesamt angeklickt wurden usw.</td>
   </tr>
   <tr>
   <td><b>Zum Öffnen klicken %</b></td>
   <td>Prozentsatz der E-Mails, die geöffnet wurden und auf die ein Link in der E-Mail geklickt wurde Auf diese Weise wird die Relevanz und der Kontext einer E-Mail gemessen, indem die Anzahl der Einzelklicks dividiert durch die Anzahl der Einzelöffnungen und anschließend durch 100 multipliziert wird, um den Prozentsatz anzuzeigen.</td>
   </tr>
   <tr>
   <td><b>Engagement-Bewertung</b></td>
   <td>Mit dem <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">Interaktionswert</a> können Sie die Effektivität Ihres Inhalts ermitteln.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Wenn Sie Interaktionsbewertung auswählen, muss der Test mindestens 24 Stunden lang ausgeführt werden. Erfahren Sie mehr über [Verständnis des Interaktionswerts](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Sie können Ihre Kriterien auch anpassen, indem Sie Benutzerspezifische Konversion auswählen und auf Bearbeiten klicken.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Mit der benutzerspezifischen Konversion können Sie jedes Ereignis mithilfe von Triggern und Filtern als Konversion auswählen.

1. Daraufhin wird ein Fenster geöffnet. Suchen Sie den gewünschten Trigger und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Definieren Sie den Trigger.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo lässt nur Trigger/Filter für Personen zu, die die E-Mail aus diesem E-Mail-Programm erhalten haben. Daher ist es nicht erforderlich, einen Filter &quot;E-Mail gesendet&quot;hinzuzufügen. Achten Sie außerdem bei der Verwendung eines E-Mail-bezogenen Triggers/Filters darauf, &quot;ist vorhanden&quot;als Operator zu verwenden.

1. Klicken Sie auf **Schließen**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Sehr gut! Jetzt ist es an der Zeit zu entscheiden, wie der Gewinner bestimmt wird.

## Gewinner benennen {#declare-winner}

1. Wählen Sie eine der beiden verfügbaren Optionen aus.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Wenn Sie einen A/B-Test vom Typ **Datum/Uhrzeit** durchführen, können Sie nur **Manuell** auswählen.

   Sobald der A/B-Test beendet ist, kann Marketo die erfolgreichste E-Mail automatisch zum geplanten Zeitpunkt senden oder Sie können die Ergebnisse überprüfen und entscheiden, welche E-Mail gesendet wird.

1. Automatisch ist großartig und ist die Standardoption. Klicken Sie einfach auf **Weiter**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Wenn Sie **Manuell** auswählen, wird der Test gesendet und gewartet, bis Sie einen Gewinner feststellen. Sie erhalten einen Bericht über die Ergebnisse.

Perfekt! Nun lassen Sie uns [den A/B-Test planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
