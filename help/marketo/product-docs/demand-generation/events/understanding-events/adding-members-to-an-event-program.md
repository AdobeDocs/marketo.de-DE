---
unique-page-id: 37355758
description: Hinzufügen von Mitgliedern zu einem Ereignis-Programm - Marketing Docs - Produktdokumentation
title: Hinzufügen von Mitgliedern zu einem Ereignis-Programm
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Hinzufügen von Mitgliedern zu einem Ereignis-Programm {#adding-members-to-an-event-program}

Dieser Artikel gilt nur für Benutzer, die Ereignis Cap oder Ereignis Goals verwenden.

>[!CAUTION]
>
>Wenn Sie eine Liste von Personen direkt in ein Ereignis-Programm importieren, wird verhindert, dass diese Datensätze in den eigentlichen Registrierungen im Bericht &quot;Zielverfolgung&quot;und im Bericht &quot;Fortschrittlichkeit bei Ereignissen&quot;gezählt werden. Befolgen Sie die unten stehenden Anweisungen, um sicherzustellen, dass Ihre Datensätze gezählt werden.

1. Erstellen Sie Personen und [fügen Sie sie einer statischen Liste](http://docs.marketo.com/x/ecKt)hinzu.
1. [Erstellen Sie eine intelligente Kampagne](http://docs.marketo.com/x/M4AR).
1. Suchen Sie in der Smart-Liste der Smart-Kampagne, die Sie in Schritt 2 erstellt haben, den Filter **Member of Liste** und fügen Sie ihn hinzu.

   ![](assets/three.png)

1. Suchen Sie die Liste, die Sie in Schritt 1 erstellt haben, und wählen Sie sie aus.
1. ![](assets/four.png)

1. Suchen und fügen Sie im Fluss den Textfluss **Change Programm Status** hinzu.
1. ![](assets/five.png)

1. Suchen und wählen Sie Ihr Ereignis-Programm aus.

   ![](assets/six.png)

1. Wählen Sie den gewünschten Status aus.

   ![](assets/seven.png)

1. Klicken Sie auf der Registerkarte Plan auf Einmal **ausführen**.
1. ![](assets/eight.png)

1. Wählen Sie **Jetzt** ausführen und klicken Sie auf **Ausführen**.
1. ![](assets/nine.png)

1. Nachdem die intelligente Kampagne ausgeführt wurde, werden die Mitglieder dem Programm hinzugefügt und zählen in den Berechnungen für die Zielverfolgung und die Ereignis-Cap-Progression.

