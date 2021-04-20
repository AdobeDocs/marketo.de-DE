---
title: priority-override-for-Trigger-Kampagnen
description: Prioritätsabweichung für Trigger-Kampagnen
exl-id: 4468868c-33d7-4b5e-b524-bfcc2785c8ce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Prioritätsabweichung für Trigger-Kampagnen

<br> 

Administratoren können Marketos festgelegte Priorität für Trigger-Kampagnen überschreiben, um Prioritäten festzulegen, die besser mit den Geschäftszielen in Einklang stehen.

>[!NOTE]
>
>Diese Funktion steht nur für Trigger-Kampagnen und für Benutzer zur Verfügung, denen die Berechtigung &quot;Trigger-Kampagne bearbeiten&quot;erteilt wurde.

>[!CAUTION]
>
>Es wird dringend empfohlen, diese Funktion auf einer begrenzten Anzahl geschäftskritischer Kampagnen zu verwenden (25 ist die empfohlene Höchstzahl). Die lockere Verwendung der Funktion auf einer großen Menge kann die Ausführung der Kampagne insgesamt beeinträchtigen.

## Priorität außer Kraft setzen

1. Klicken Sie in der Kampagne Ihres Triggers auf die Registerkarte **[!UICONTROL Plan]** und dann auf **[!UICONTROL Priorität außer Kraft setzen]**.

   ![Bild eins](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Wählen Sie eine neue Prioritätsstufe aus der Dropdownliste. Klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![Bild zwei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Bild drei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Sie können die Standardpriorität Ihrer Kampagne in der [!UICONTROL Kampagne-Warteschlange] unter [!UICONTROL Marketing-Aktivitäten] Ansicht. Um die Ausführungsrate zu erhöhen, sollten Sie die Priorität Ihrer Kampagne auf eine Ebene höher als die Standardeinstellung setzen.
>* Die Priorität der Benutzereinstellung gilt nur für neue Personen, die sich für die Kampagne qualifizieren. Personen, die sich bereits in der Warteschlange befinden, sind davon nicht betroffen.


## Priorität zurücksetzen

1. Um die Systemstandardpriorität zurückzusetzen, wechseln Sie zur Registerkarte **[!UICONTROL Plan]** in der Kampagne Ihres Triggers und klicken Sie auf **[!UICONTROL Kampagne zurücksetzen]**.

   ![Bild vier](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Zurücksetzen]**.

   ![Bild fünf](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Prioritätsüberschreibungen und -rückgaben werden im Audit-Protokoll erfasst. Sie können den [Prüfpfad](https://docs.marketo.com/x/GZ2t) durch den [!UICONTROL Admin]-Bereich im klassischen Erlebnis Ansicht haben.

## Zugriff auf Förderpriorität außer Kraft setzen

>[!CAUTION]
>
>Nur Administratoren oder Benutzer mit Administratorrechten sollten über die Priorität &quot;Kampagne&quot;verfügen, um den Zugriff zu überschreiben.

1. Klicken Sie im Bereich [!UICONTROL Admin] auf **[!UICONTROL Benutzer und Rollen]**.

   ![Bild sechs](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Rollen]**, wählen Sie den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie dann auf **[!UICONTROL Rolle bearbeiten]**.

   ![Bild sieben](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Markieren Sie unter [!UICONTROL Zugriff auf Marketing-Aktivitäten] **[!UICONTROL Kampagne des Triggers bearbeiten]**. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![Bild acht](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Priorität der Kampagne der Ansicht in Marketo Classic

Sie können die Priorität der Kampagne im Erlebnis [!DNL Classic] durch Klicken auf die Registerkarte **[!UICONTROL Planen]** in einer Trigger-Kampagne festlegen.

![Bild neun](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>Die Priorität im Erlebnis [!DNL Classic] ist nur Ansicht. Das Ändern oder Zurücksetzen der Priorität der Kampagne ist nur über Marketo Sky verfügbar.
