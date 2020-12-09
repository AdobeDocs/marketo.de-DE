---
title: priority-override-for-trigger-Kampagnen
description: Prioritätsabweichung für Auslöser-Kampagnen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Prioritätsabweichung für Auslöser-Kampagnen

<br> 

Administratoren können Marketos festgelegte Priorität für auslösende Kampagnen außer Kraft setzen, um Prioritäten festzulegen, die besser mit Geschäftszielen übereinstimmen.

>[!NOTE]
>
>Diese Funktion steht nur für Trigger-Kampagnen und für Benutzer zur Verfügung, denen die Berechtigung &quot;Kampagne bearbeiten&quot;erteilt wurde.

>[!CAUTION]
>
>Es wird dringend empfohlen, diese Funktion auf einer begrenzten Anzahl geschäftskritischer Kampagnen zu verwenden (25 ist die empfohlene Höchstzahl). Die lockere Verwendung der Funktion auf einer großen Menge kann die Ausführung der Kampagne insgesamt beeinträchtigen.

## Priorität außer Kraft setzen

1. Klicken Sie in der Kampagne des Auslösers auf die Registerkarte **[!UICONTROL Plan]** und dann auf Priorität **[!UICONTROL außer Kraft setzen]**.

   ![Bild eins](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Wählen Sie eine neue Prioritätsstufe aus der Dropdownliste. Klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![Bild zwei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Bild drei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Sie können die Standardpriorität Ihrer Kampagne in der [!UICONTROL Kampagne-Warteschlange] unter [!UICONTROL Marketing-Aktivitäten]Ansicht haben. Um die Ausführungsrate zu erhöhen, sollten Sie die Priorität Ihrer Kampagne auf eine Ebene höher als die Standardeinstellung setzen.
>* Die Priorität der Benutzereinstellung gilt nur für neue Personen, die sich für die Kampagne qualifizieren. Personen, die sich bereits in der Warteschlange befinden, sind davon nicht betroffen.


## Priorität zurücksetzen

1. Wenn Sie die Systemstandardpriorität zurücksetzen möchten, wechseln Sie zur Registerkarte &quot; **[!UICONTROL Plan]** &quot;in der Auslöseansicht und klicken Sie auf &quot;Kampagne **[!UICONTROL zurücksetzen&quot;]**.

   ![Bild vier](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Zurücksetzen]** .

   ![Bild fünf](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Prioritätsüberschreibungen und -rückgaben werden im Audit-Protokoll erfasst. Sie können den [Prüfpfad](https://docs.marketo.com/x/GZ2t) im Classic-Erlebnis über den [!UICONTROL Admin] -Bereich Ansicht haben.

## Zugriff auf Förderpriorität außer Kraft setzen

>[!CAUTION]
>
>Nur Administratoren oder Benutzer mit Administratorrechten sollten über die Priorität &quot;Kampagne&quot;verfügen, um den Zugriff zu überschreiben.

1. Klicken Sie im Bereich [!UICONTROL Admin] auf **[!UICONTROL Benutzer und Rollen]**.

   ![Bild sechs](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Rollen]** , wählen Sie den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie dann auf Rolle **[!UICONTROL bearbeiten]**.

   ![Bild sieben](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Aktivieren Sie unter [!UICONTROL Zugriff auf Marketing-Aktivitäten]die Option Auslöserpriorität **[!UICONTROL bearbeiten]**. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![Bild acht](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Priorität der Kampagne von Ansichten in Marketing Classic

Sie können die Priorität der Ansicht der Kampagne im [!DNL Classic] Erlebnis festlegen, indem Sie in einer Auslöser-Kampagne auf die Registerkarte **[!UICONTROL Plan]** klicken.

![Bild neun](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>Die Priorität des [!DNL Classic] Erlebnisses ist nur Ansicht. Das Ändern oder Zurücksetzen der Priorität der Kampagne ist nur über Marketo Sky verfügbar.
