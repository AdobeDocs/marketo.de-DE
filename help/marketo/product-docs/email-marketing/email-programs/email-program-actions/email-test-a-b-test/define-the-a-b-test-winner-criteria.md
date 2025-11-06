---
unique-page-id: 2359545
description: Definieren der Kriterien für den A/B-Testsieger - Marketo-Dokumente - Produktdokumentation
title: Definieren der Kriterien für den A/B-Testsieger
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: c80d25aeafe2314fcff1d99359ff146c88acad06
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 21%

---

# Definieren der Kriterien für den A/B-Testsieger {#define-the-a-b-test-winner-criteria}

Beim [Hinzufügen eines A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}Tests zu Ihrem E-Mail-Programm müssen Sie einen Testtyp auswählen, [den A/B-Test planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"} und dann die Kriterien für den Gewinner definieren. So entscheiden Sie, welche E-Mail gewinnt.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Gewinnerkriterien {#winner-criteria}

1. Die Standardoptionen **[!UICONTROL Gewinnerkriterien]** werden zuerst aufgeführt.

   ![](assets/define-the-a-b-test-winner-criteria-1.png)

   <table>
   <tr>
   <td><b>[!UICONTROL wird geöffnet]</b></td>
   <td>Ein geöffnetes registriert beim Herunterladen von Bildern in eine E-Mail. Auch wenn Sie kein Bild einbeziehen, fügt Marketo standardmäßig ein einzelnes Tracking-Pixel in alle HTML-E-Mails ein.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Klicks]</b></td>
   <td>Standardmäßig sind Tracking-Funktionen für Links in E-Mails integriert, sodass Sie sehen können, wer auf welchen Link geklickt hat, wie viele Links insgesamt angeklickt wurden usw.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Zum Öffnen klicken] %</b></td>
   <td>Prozentsatz der E-Mails, die geöffnet wurden und bei denen auf einen Link in der Nachricht geklickt wurde. Dabei werden Relevanz und Kontext einer E-Mail gemessen. Hierzu wird die Anzahl der Einzelklicks durch die Anzahl der Einzelöffnungen dividiert und mit 100 multipliziert, um den Wert als Prozentsatz anzuzeigen.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Engagement Score]</b></td>
   <td>Der <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">Interaktionswert</a> hilft Ihnen bei der Bestimmung der Effektivität Ihrer Inhalte.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Wenn Sie Engagement Score auswählen, muss der Test mindestens 24 Stunden lang ausgeführt werden. Weitere Informationen über [Verstehen des Interaktionswerts](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Sie können Ihre Kriterien auch anpassen, indem Sie **[!UICONTROL Benutzerdefinierte Konversion]** auswählen und auf **[!UICONTROL Bearbeiten]** klicken.

   ![](assets/define-the-a-b-test-winner-criteria-2.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Konversion ermöglicht es Ihnen, jedes Ereignis als Konversion auszuwählen, indem Sie Trigger und Filter verwenden.

1. Ein Fenster wird geöffnet. Suchen Sie den Trigger Ihrer Wahl und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/define-the-a-b-test-winner-criteria-3.png)

1. Definieren Sie den Trigger.

   ![](assets/define-the-a-b-test-winner-criteria-4.png)

   >[!IMPORTANT]
   >
   >Marketo lässt nur Trigger/Filter für Personen zu, die die E-Mail von diesem E-Mail-Programm erhalten haben. Daher ist es nicht erforderlich, den Filter „Wurde E-Mail gesendet“ hinzuzufügen. Darüber hinaus sollten Sie bei der Verwendung eines E-Mail-bezogenen Triggers/Filters „is any“ als Operator verwenden.

1. Schließen Sie das neu geöffnete Fenster (oder die neu geöffnete Registerkarte). Die Smart-Liste wird automatisch gespeichert.

Jetzt ist es an der Zeit zu entscheiden, wie der Gewinner bestimmt wird.

## Gewinner benennen {#declare-winner}

1. Wählen Sie eine der beiden verfügbaren Optionen aus.

   ![](assets/define-the-a-b-test-winner-criteria-5.png)

   >[!NOTE]
   >
   >Wenn Sie einen A/B **Test mit Datum/Uhrzeit**, können Sie nur &quot;**[!UICONTROL &quot;]**.

   Sobald der A/B-Test abgeschlossen ist, kann Marketo die erfolgreichste E-Mail automatisch zum geplanten Zeitpunkt senden. Alternativ können Sie die Ergebnisse überprüfen und entscheiden, welche E-Mail zu welchem Zeitpunkt gesendet wird.

1. Automatisch ist genial und ist die Standardoption. Klicken Sie einfach **[!UICONTROL Weiter]**.

   ![](assets/define-the-a-b-test-winner-criteria-6.png)

   >[!TIP]
   >
   >Wenn Sie **[!UICONTROL Manuell]** wählen, wird der Test gesendet und Sie müssen warten, bis Sie einen Gewinner bestimmen. Sie erhalten einen Bericht über die Ergebnisse.

Planen wir nun [den A/B-Test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
