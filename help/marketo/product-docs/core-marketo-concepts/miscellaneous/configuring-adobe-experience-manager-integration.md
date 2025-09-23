---
unique-page-id: 30081815
description: Konfigurieren der Adobe Experience Manager-Integration - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren der Integration in Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 7%

---

# Konfigurieren der Integration in Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Konfigurieren Sie Adobe Experience Manager (AEM), damit Sie auf AEM-Assets zugreifen, sie auswählen und in Marketo Engage Design Studio importieren können.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!IMPORTANT]
>
>* Diese Integration funktioniert nur mit On-Premise-Implementierungen von AEM und wird bei AEM Cloud Service-Implementierungen nicht unterstützt.
>
>* Derzeit wird diese Funktion nur in Firefox vollständig unterstützt. Er wird in Safari nicht unterstützt und funktioniert möglicherweise nicht in der neuesten Version von Chrome, je nach den SameSite-Cookie-Einstellungen.

1. Navigieren Sie zur Adobe Experience Manager (die URL ist spezifisch für Ihr Unternehmen).

   ![](assets/one.png)

1. Sie können sich mit Adobe anmelden oder lokal anmelden. In diesem Beispiel melden wir uns lokal an.

   ![](assets/two.png)

1. Klicken Sie **[!UICONTROL Tools]** auf **[!UICONTROL Vorgänge]** und wählen Sie **[!UICONTROL Web-Konsole]** aus.

   ![](assets/2a.png)

1. Suchen Sie in Ihrem Browser (Strg+F unter Windows, Befehl+F unter Mac) nach &quot;[!UICONTROL Adobe Granite Cross-Origin Resource Sharing Policy]&quot;.

   ![](assets/three.png)

1. Klicken Sie auf das **+** rechts.

   ![](assets/four.png)

1. Geben Sie **[!UICONTROL Textfeld „Zulässige Ursprünge (Regexp]** ein und klicken Sie auf `https://.*\.marketo\.com`Speichern **&#x200B;**.

   ![](assets/five-psd.png)

1. Klicken Sie oben auf der Seite in der Kopfzeile auf **[!UICONTROL Web-Konsole]** und wählen Sie **[!UICONTROL Systeminformationen]** aus.

   ![](assets/six.png)

1. Klicken Sie unter „Server Information“ auf die **[!UICONTROL Neustart]**-Schaltfläche.

   ![](assets/seven.png)

1. Klicken **[!UICONTROL zur Bestätigung]** OK.

   ![](assets/eight.png)

1. Klicken Sie in Marketo Engage auf **[!UICONTROL Admin]**.

   ![](assets/nine.png)

1. Wählen Sie unter Integration die Option **[!UICONTROL Adobe Experience Manager]** aus.

   ![](assets/ten.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/eleven.png)

1. Geben Sie Ihre AEM-URL ein und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/twelve.png)
