---
description: So sperren Sie gesendete Spam-Formulare - Marketo Dokumente - Produktdokumentation
title: So sperren Sie gesendete Spam-Formulare
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# So sperren Sie Spam-Formularübermittlungen {#how-to-block-spam-form-submissions}

Häufig können Formularübermittlungen mit einer ungültigen oder fehlenden Prüfsumme (normalerweise von Bots) falsche Statistiken ergeben. Hier ist, wie man das verhindert.

>[!CAUTION]
>
>Diese Funktion lehnt Formularübermittlungen ab, die mit programmatischen POSTs an den Endpunkt leadCapture/save2 gesendet wurden. Wenn Ihr Unternehmen eine Integration verwendet, die Formulare mit dieser Methode an Marketo sendet, blockiert die Aktivierung dieser Funktion diese Übermittlungen. Die Verwendung von &quot;leadCapture/save2&quot;als API oder die Ausführung programmatischer Formularübermittlungen direkt an die Variable wird nicht unterstützt und ist verboten. Vergewissern Sie sich, dass Ihr Unternehmen nur Formulare einreicht mit: Formularelemente, Code für eingebettete Formulare, Forms2.js-API oder die REST-API für das Senden von Formularen.

1. Klicken Sie auf **Admin**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Klicken Sie auf **Schatztruhe**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. Klicken Sie neben **Personenerfassung - Ungültige Prüfsummenwerte ablehnen** auf **Bearbeiten**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Aktivieren Sie das Kontrollkästchen **Aktiviert** und klicken Sie auf **Speichern**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>Wenn Sie diese Funktion aktivieren, sehen Sie möglicherweise einen Abbruch in der Aktivität, wenn falsche Zahlen herausgefiltert werden.
