---
unique-page-id: 4720218
description: Implementieren von RTP mit Adobe Tag Manager - Marketo Docs - Produktdokumentation
title: Implementieren von RTP mit Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementieren von RTP mit Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Melden Sie sich bei Ihrem RTP-Konto an.

1. Navigieren Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 4 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Suchen Sie unter Domäne die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Melden Sie sich bei Ihrem Dynamic Tag Manager-Konto an ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Navigieren Sie zu **Dashboard.** Klicken Sie auf die entsprechende Webeigenschaft.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Navigieren Sie zu **Regeln** klicken **Neue Regel erstellen**.

1. Füllen Sie Folgendes aus:

   1. Name: **Marketo RTP**
   1. Bedingungen (Reduzieren) : Trigger-Regel unter - **Seitenanfang**
   1. JavaScript (Reduzieren): Klicken **Neues Skript hinzufügen**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Rufen Sie das neue Tag auf: **Marketo RTP-Tag**

1. Entfernen Sie den folgenden Code aus dem RTP-Tag

   * `<script type='text/javascript'>`
   * `</script>`

1. Fügen Sie das RTP-JavaScript-Tag ein.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Achten Sie darauf, alle Tags zu entfernen und nur das Skript selbst zu lassen (nein `<script type='text/javascript'>` , `</script>` )

1. Klicks **Code speichern** im Skript-Editor und **Regel speichern** im Regeleditor.

1. Suchen Sie im Bereich Regeln die Marketo RTP-Seitenladeregel und innerhalb der Variablen **Aktionen** Dropdown-Auswahl **Aktivieren von Regeln**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Überprüfen** dass sie auf allen Seiten einschließlich Landingpages und Subdomänen angezeigt wird.

   Klicken Sie mit der rechten Maustaste auf die Seiten Ihrer Website. Navigieren Sie zu **Inspect-Element**, klicken Sie auf **Netzwerk**, Suche: **RTP**.
