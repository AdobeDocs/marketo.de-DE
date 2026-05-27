---
unique-page-id: 2360217
description: Wie Sie in der Umsatzzyklusanalyse Optionen für Erstkontakt- und Multitouch-Attribution, Lead-Konversion und Marketing-beeinflusste Opportunities festlegen.
title: Ändern der Attributionseinstellungen für Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 5%

---

# Ändern der Attributionseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, wie Marketo Kontakte mit Opportunities für Erstkontakt- und Mehrfachkontakt-Attribution, Lead-Konversionsmetriken und der Marketing-beeinflussten Opportunity-Markierung verknüpft.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicken Sie **[!UICONTROL Umsatzzyklusanalyse]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicken Sie auf den **[!UICONTROL Bearbeiten]**-Link unter **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Durch Ändern dieser Einstellung werden keine Marketo-Daten geändert. Vielmehr ändert sich dadurch die Ausführung Ihrer Berichte. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Explicit]**: Nur Kontakte mit Rollen (Standard).
   >
   >**[!UICONTROL Hybrid]**: Kontakte mit Rollen, falls verfügbar. Wenn keine verfügbar sind, werden alle Kontakte in Konten verwendet.
   >
   >**[!UICONTROL Implizit]**: Alle Kontakte unabhängig von der Rolle.

>[!CAUTION]
>
>Bei Verwendung von **[!UICONTROL implizit]** prüft Marketo immer alle mit dem Konto verknüpften Kontakte, unabhängig von der Rolle. **Marketo empfiehlt dringend die Verwendung [!UICONTROL expliziten] Modus**. Die Verwendung von [!UICONTROL Implicit] kann zu falsch positiven Ergebnissen führen, d. h. zu Personen, die eine Opportunity guthaben, obwohl sie keinen echten Einfluss auf die Opportunity haben. Verwenden Sie [!UICONTROL implizit] mit Vorsicht.
