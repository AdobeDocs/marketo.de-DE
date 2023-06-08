---
unique-page-id: 10617187
description: Grundlegendes zu Datenschutzeinstellungen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Datenschutzeinstellungen
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Grundlegendes zu Datenschutzeinstellungen {#understanding-privacy-settings}

## Überblick {#overview}

Marketo bietet Marketing-Experten die Möglichkeit, die Zustimmung von Webbesuchern zur Nachverfolgung zu erhalten. Es gibt zwei Möglichkeiten, sich abzumelden, oder Sie können entscheiden, von einer anonymisierten IP verfolgt zu werden.

* Webbesucher wählen die Funktion &quot;Nicht verfolgen&quot;(DNT) in ihrem Browser aus (und der Marketing-Experte berücksichtigt die Anforderung des Webbesuchers, &quot;Nicht verfolgen&quot;zu verwenden).
* Webbesucher verwenden ein Opt-out-Cookie, das von einem Marketingspezialisten auf einer Website bereitgestellt wird

Oder der Marketing-Experte kann Benutzer verfolgen, aber eine anonymisierte IP verwenden.

Diese Methoden können sich auf den Wert und die Funktionalität von Marketo in bestimmten Bereichen auswirken. Wenn der Marketing-Experte jedoch _nicht_ Änderungen an der Konfiguration von Marketo vornehmen, bleiben die Marketo-Funktionen unverändert.

## Browsereinstellungen für &quot;Nicht verfolgen&quot; {#browser-settings-for-do-not-track}

Webbesucher können ihren Browser so einstellen, dass das Tracking durch eine beliebige Website verhindert wird, indem sie &quot;Do Not Track&quot;(DNT) auswählen. Dies verhindert das Tracking für diesen bestimmten Browser und Gerät. Vollständige Informationen finden Sie in den Datenschutzeinstellungen des Browsers.

In [!DNL Munchkin], kann ein Marketing-Experte [Entscheiden Sie, ob Sie die DNT-Einstellung des Browsers unterstützen oder ignorieren möchten.](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Bei der Web-Personalisierung kann ein Marketing-Experte entscheiden, ob [Unterstützung oder Ignorieren der DNT-Einstellung des Browsers](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Abmelden von einer bestimmten Website {#opt-out-from-a-specific-website}

Sie können Website-Besuchern auch erlauben, das Website-Tracking von Ihrer Website abzuwählen, unabhängig davon, ob **Browser nicht verfolgen** -Einstellungen konfiguriert werden. Dadurch kann der Site-Besucher seine Tracking-Voreinstellungen direkt auf Ihrer Website festlegen.

Dazu müssen Sie einen Parameter zu einem Ausschluss-Link auf einer Webseite hinzufügen, die [!DNL Munchkin] Tracking aktiviert. Dabei kann es sich um eine beliebige Webseite handeln, der Webseitenlink muss jedoch den folgenden Parameter enthalten:

?marketo_opt_out=true

Im Folgenden finden Sie Beispiele für eine Webseite mit einem Ausschluss-Link und eine Landingpage für , nachdem auf den Link geklickt wurde. Deine wird anders sein.

Hier ist eine Webseite mit einer Schaltfläche mit dem Parameter &quot;?marketo_opt_out=true&quot; im Ausschluss-Link.

![](assets/understanding-privacy-settings-1.png)

Sie können eine Landingpage erstellen und veröffentlichen, wenn auf Ihren Link mit dem Parameter &quot;?marketo_opt_out=true&quot;geklickt wird.

![](assets/understanding-privacy-settings-2.png)

Wenn auf den Link geklickt wird, fügt Marketo ein Cookie mit dem Namen **mkto_opt_out** zum Browser des Besuchers, der deaktiviert [!DNL Munchkin] Tracking für den Site-Besucher, der auf den Link mit dem obigen Parameter klickt.

Um zu überprüfen, ob das Cookie platziert werden kann, stellen Sie sicher, dass Sie ein Cookie-Lead sind, und klicken Sie auf den Link. Überprüfen Sie dann Ihre Browser-Cookies, um sicherzustellen, dass die Variable **mkto_opt_out** -Cookie hinzugefügt wurde.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Dies funktioniert derzeit nur mit [!DNL Munchkin] Versionen 152 und höher.

## Opt In {#opt-in}

Marketingexperten können den Benutzern die Möglichkeit geben, sich über die Funktionen von Marketo in E-Mails, Formularen, Landingpages und anderen Methoden anzumelden.

## Tracking mit einer anonymisierten IP {#tracking-using-an-anonymized-ip}

Marketingexperten können den Datenschutz wahren, indem sie Benutzer mit einer anonymisierten IP-Adresse verfolgen. Fügen Sie dazu diesen Code zum RTP hinzu oder [!DNL Munchkin] JavaScript, das in die Website eingebettet ist.

* Für [!DNL Munchkin], fügen Sie einfach {&quot;anonymizeIP&quot;,true} zur init-Funktion hinzu.

  >[!NOTE]
  >
  >Die Verwendung dieses Parameters erfordert, dass [!DNL Munchkin] V2 aktiviert sein. Wenden Sie sich an die [Marketo-Support](https://nation.marketo.com/community/support_solutions).

* Fügen Sie für Web Personalization (RTP) Folgendes zum JavaScript hinzu:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
