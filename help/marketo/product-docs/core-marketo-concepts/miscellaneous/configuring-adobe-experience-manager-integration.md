---
unique-page-id: 30081815
description: Konfigurieren der Adobe Experience Manager-Integration - Marketo Docs - Produktdokumentation
title: Konfigurieren der Adobe Experience Manager-Integration
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Konfigurieren der Adobe Experience Manager-Integration {#configuring-adobe-experience-manager-integration}

Konfigurieren Sie AEM, damit Sie auf AEM Assets zugreifen, sie auswählen und in Marketo Design Studio importieren können.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!CAUTION]
>
>Diese Funktion wird derzeit nur in Firefox vollständig unterstützt. Sie wird in Safari nicht unterstützt und funktioniert möglicherweise nicht in der neuesten Version von Chrome, je nach Ihren SameSite-Cookie-Einstellungen.

1. Navigieren Sie zur Adobe Experience Manager (die URL ist unternehmensspezifisch).

   ![](assets/one.png)

1. Sie können sich mit Adobe anmelden oder sich lokal anmelden. In diesem Beispiel werden wir uns lokal anmelden.

   ![](assets/two.png)

1. In **Instrumente** klicken **Aktivitäten** und wählen Sie **Web-Konsole**.

   ![](assets/2a.png)

1. Suchen Sie in Ihrem Browser (Strg+f unter Windows, Befehl+F unter Mac) nach &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot;.

   ![](assets/three.png)

1. Klicken Sie auf **+** rechts.

   ![](assets/four.png)

1. Im **Zulässiger Ursprung (Regexp)** Textfeld, Eingabe `https://.*\.marketo\.com` und klicken Sie auf **Speichern**.

   ![](assets/five-psd.png)

1. Klicken Sie in der Kopfzeile oben auf der Seite auf **Web-Konsole** und wählen Sie **Systeminformationen**.

   ![](assets/six.png)

1. Klicken Sie unter &quot;Serverinformationen&quot;auf die **Neu starten** Schaltfläche.

   ![](assets/seven.png)

1. Klicken **OK** zur Bestätigung.

   ![](assets/eight.png)

1. Klicken Sie in Marketo Classic auf **Admin**.

   ![](assets/nine.png)

1. Wählen Sie unter Integration die Option **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Klicken **Bearbeiten**.

   ![](assets/eleven.png)

1. Geben Sie Ihre AEM-URL ein und klicken Sie auf **OK**.

   ![](assets/twelve.png)

   Du bist ganz fertig! Sie können jetzt [Importieren AEM Assets in Design Studio in Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
