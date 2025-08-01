---
unique-page-id: 4720218
description: Implementieren von RTP mit Adobe Tag Manager - Marketo-Dokumente - Produktdokumentation
title: Implementieren von RTP mit Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Implementieren von RTP mit Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Um Ihr RTP-Tag zu implementieren, befolgen Sie die folgenden Installationsanweisungen:

1. Melden Sie sich bei Ihrem RTP-Konto an.

1. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 4 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Suchen Sie unter [!UICONTROL Domain] die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Melden Sie sich bei Ihrem [!DNL Dynamic Tag Manager] Konto an ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Navigieren Sie zu **[!UICONTROL Dashboard].** Klicken Sie auf die entsprechende Web-Eigenschaft.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Navigieren Sie zu **[!UICONTROL Regeln]** und klicken Sie auf **[!UICONTROL Neue Regel erstellen]**.

1. Füllen Sie Folgendes aus

   1. [!UICONTROL Name]: **Marketo RTP**
   1. [!UICONTROL Bedingungen] (reduzieren) : Trigger-Regel bei - **[!UICONTROL Seitenanfang]**
   1. [!UICONTROL JavaScript] (reduzieren): klicken Sie auf **[!UICONTROL Neues Skript hinzufügen]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Rufen Sie das neue Tag auf: **Marketo RTP-Tag**

1. Entfernen Sie den folgenden Code aus dem [!UICONTROL RTP-Tag]

   * `<script type='text/javascript'>`
   * `</script>`

1. Fügen Sie das RTP-JavaScript-Tag ein.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Entfernen Sie alle Tags und belassen Sie nur das Skript selbst (keine `<script type='text/javascript'>` , `</script>` )

1. Klicken Sie **[!UICONTROL Skript]** Editor auf „Code speichern“ und **[!UICONTROL Regel speichern]** im Regeleditor.

1. Suchen Sie im Bedienfeld Regeln die Marketo-RTP-Seitenladeregel und wählen Sie in der Dropdown-Liste **[!UICONTROL Aktionen]** die Option **[!UICONTROL Regeln aktivieren]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Überprüfen]** ob es auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains.

   Sie können dies tun, indem Sie mit der rechten Maustaste auf die Seiten Ihrer Website klicken. Navigieren Sie zu **[!UICONTROL Element überprüfen]** und klicken Sie auf **[!UICONTROL Netzwerk]**, Suche: **RTP**.
