---
unique-page-id: 4720218
description: Implementierung von RTP mit Adobe Tag Manager - Marketing Docs - Produktdokumentation
title: Implementieren von RTP mit Adobe Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Implementieren von RTP mit Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Befolgen Sie zur Implementierung Ihres RTP-Tags die Installationsanweisungen unten:

1. Melden Sie sich bei Ihrem RTP-Konto an.
1. Gehen Sie zu **Kontoeinstellungen.**

   Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 4 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag** generieren.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Melden Sie sich bei Ihrem dynamischen Tag-Manager-Konto an ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).
1. Wechseln Sie zu **Dashboard.** Klicken Sie auf die entsprechende Webeigenschaft.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Gehen Sie zu **Regeln,** Klicken Sie auf **Neue Regel erstellen.**

1. Füllen Sie die folgenden Felder aus

   1. Name: **Marketo RTP**
   1. Bedingungen (Zusammenbruch): Auslöserregel bei - **Anfang der Seite**
   1. JavaScript (Reduzieren): Klicken Sie auf **Hinzufügen Neues Skript**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Rufen Sie das neue Tag auf: **Marketo-RTP-Tag**
1. Entfernen Sie den folgenden Code aus dem RTP-Tag

   * `<script type='text/javascript'>`
   * `</script>`

1. Fügen Sie das RTP JavaScript-Tag ein.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Achten Sie darauf, alle Tags zu entfernen und nur das Skript selbst zu belassen (no `<script type='text/javascript'>` , `</script>` ).

1. Klicken Sie im Skript-Editor auf **Code speichern** und im Regeleditor auf **Regel speichern**.

1. Suchen Sie im Regelbedienfeld die Marketo RTP-Seitenladeregel und wählen Sie im Dropdownmenü **Aktionen** die Option Regeln aktivieren **aus.**

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Vergewissern Sie** sich, dass er auf allen Seiten einschließlich Landingpages und Subdomänen angezeigt wird.

   Dazu klicken Sie mit der rechten Maustaste auf die Seiten Ihrer Website. Gehen Sie zu **Inspect Element**, klicken Sie auf **Netzwerk, **Suche: **RTP**.
