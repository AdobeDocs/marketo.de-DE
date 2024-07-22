---
unique-page-id: 30081815
description: Konfigurieren der Adobe Experience Manager-Integration - Marketo Docs - Produktdokumentation
title: Konfigurieren der Adobe Experience Manager-Integration
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Konfigurieren der Adobe Experience Manager-Integration {#configuring-adobe-experience-manager-integration}

Konfigurieren Sie Adobe Experience Manager (AEM), damit Sie auf AEM Assets zugreifen, sie auswählen und in Marketo Engage Design Studio importieren können.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!IMPORTANT]
>
>* Diese Integration funktioniert nur mit On-Premise-Implementierungen von AEM und wird nicht für AEM Cloud Service-Implementierungen unterstützt.
>
>* Diese Funktion wird derzeit nur in Firefox vollständig unterstützt. Sie wird in Safari nicht unterstützt und funktioniert möglicherweise nicht in der neuesten Version von Chrome, je nach Ihren SameSite-Cookie-Einstellungen.

1. Navigieren Sie zur Adobe Experience Manager (die URL ist unternehmensspezifisch).

   ![](assets/one.png)

1. Sie können sich mit Adobe anmelden oder sich lokal anmelden. In diesem Beispiel werden wir uns lokal anmelden.

   ![](assets/two.png)

1. Klicken Sie in **[!UICONTROL Tools]** auf **[!UICONTROL Vorgänge]** und wählen Sie **[!UICONTROL Web-Konsole]** aus.

   ![](assets/2a.png)

1. Suchen Sie in Ihrem Browser (Strg+f unter Windows, Befehl+F unter Mac) nach &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot;.

   ![](assets/three.png)

1. Klicken Sie auf das Symbol **+** rechts.

   ![](assets/four.png)

1. Geben Sie im Textfeld **[!UICONTROL Zulässiger Ursprung (Regexp)]** den Wert `https://.*\.marketo\.com` ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/five-psd.png)

1. Klicken Sie in der Kopfzeile oben auf der Seite auf **[!UICONTROL Web-Konsole]** und wählen Sie **[!UICONTROL Systeminformationen]** aus.

   ![](assets/six.png)

1. Klicken Sie unter &quot;Server Information&quot;auf die Schaltfläche **[!UICONTROL Neu starten]** .

   ![](assets/seven.png)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL OK]** .

   ![](assets/eight.png)

1. Klicken Sie unter Marketo Engage auf **[!UICONTROL Admin]**.

   ![](assets/nine.png)

1. Wählen Sie unter &quot;Integration&quot;die Option **[!UICONTROL Adobe Experience Manager]**.

   ![](assets/ten.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/eleven.png)

1. Geben Sie Ihre AEM-URL ein und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/twelve.png)
