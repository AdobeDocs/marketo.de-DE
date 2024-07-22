---
unique-page-id: 4720145
description: Implementieren von RTP mit dem Google Tag Manager - Marketo Docs - Produktdokumentation
title: Implementieren von RTP mit dem Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Implementieren von RTP mit dem Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Befolgen Sie zur Implementierung Ihres RTP-Tags die unten stehenden Installationsanweisungen.

1. Melden Sie sich bei Ihrem Google Tag Manager-Konto an.

1. Fügen Sie ein neues Tag > Tag-Konfigurationen > Benutzerdefiniertes HTML-Tag** hinzu.** Rufen Sie es auf **RTP**.

1. Melden Sie sich bei Ihrem RTP-Konto an**.**

1. Wechseln Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 6 fort.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es in das neue **benutzerdefinierte HTML-Tag** ein, das Sie erstellt haben (Schritt 1).

1. Klicken Sie auf **+Regel zum Auslösen des Tags hinzufügen**. Wählen Sie **Alle Seiten** aus.

1. Klicken Sie auf **Speichern** und [veröffentlichen Sie die neue Version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vergewissern Sie sich, dass sie auf allen Seiten angezeigt wird, einschließlich Landingpages und Sub-Domains.

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Inspect-Element**, suchen Sie nach **RTP** , um das Tag zu finden.
