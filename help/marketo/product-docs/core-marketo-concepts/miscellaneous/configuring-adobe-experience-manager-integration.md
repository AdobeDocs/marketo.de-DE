---
unique-page-id: 30081815
description: Adobe Experience Manager-Integration konfigurieren - Marketing Docs - Produktdokumentation
title: Adobe Experience Manager-Integration konfigurieren
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Adobe Experience Manager-Integration konfigurieren {#configuring-adobe-experience-manager-integration}

Konfigurieren Sie AEM, damit Sie auf AEM Assets zugreifen, sie auswählen und sie in das Design Studio von Marketo importieren können.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!CAUTION]
>
>Diese Funktion wird derzeit nur in Firefox vollständig unterstützt. Es wird in Safari nicht unterstützt, und es funktioniert möglicherweise nicht in der neuesten Version von Chrome (Version 80), abhängig von Ihren Einstellungen für SameSite-Cookies.

1. Navigieren Sie zum Adobe Experience Manager (die URL ist spezifisch für Ihre Firma).

   ![](assets/one.png)

1. Sie können sich mit Adobe anmelden oder sich lokal anmelden. In diesem Beispiel melden wir uns lokal an.

   ![](assets/two.png)

1. Klicken Sie unter **Tools** auf **Vorgänge** und wählen Sie **Webkonsole**.

   ![](assets/2a.png)

1. Suchen Sie in Ihrem Browser (Strg+F unter Windows, Cmd+F unter Mac) nach &quot;Adobe Granite Cross-Herkunft Resource Sharing Policy&quot;.

   ![](assets/three.png)

1. Klicken Sie auf das Symbol **+** rechts.

   ![](assets/four.png)

1. Geben Sie im Textfeld **Zulässige Herkünfte (Regexp)** `https://.*\.marketo\.com` ein und klicken Sie auf **Speichern**.

   ![](assets/five-psd.png)

1. Klicken Sie in der Kopfzeile oben auf der Seite auf **Webkonsole** und wählen Sie **Systeminformationen**.

   ![](assets/six.png)

1. Klicken Sie unter &quot;Serverinformationen&quot;auf die Schaltfläche **Neustart**.

   ![](assets/seven.png)

1. Klicken Sie zur Bestätigung auf **OK**.

   ![](assets/eight.png)

1. Klicken Sie in Marketing Classic auf **Admin**.

   ![](assets/nine.png)

1. Wählen Sie unter Integration **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/eleven.png)

1. Geben Sie Ihre AEM-URL ein und klicken Sie auf **OK**.

   ![](assets/twelve.png)

   Du bist alle fertig! Sie können jetzt [AEM Assets in das Design Studio in Marketo Sky](https://help.marketo.com/hc/en-us/articles/360036765993) importieren.
