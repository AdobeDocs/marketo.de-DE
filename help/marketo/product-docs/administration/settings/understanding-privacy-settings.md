---
unique-page-id: 10617187
description: Datenschutzeinstellungen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Datenschutzeinstellungen
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: eccf4a66f5d3c581a82a363918b40ae37aa73576
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Grundlegendes zu Datenschutzeinstellungen {#understanding-privacy-settings}

## Überblick {#overview}

Marketo bietet Marketing-Fachleuten eine Möglichkeit, das Einverständnis der Web-Besucher einzuholen, um sie nachzuverfolgen. Es gibt zwei Möglichkeiten, sich abzumelden, oder Sie können wählen, ob Sie von anonymisierter IP verfolgt werden möchten.

* Web-Besuchende wählen die Funktion „Nicht verfolgen“ (DNT) in ihrem Browser aus (und der Marketer berücksichtigt die Anfrage des Web-Besuchers nach „Nicht verfolgen„)
* Web-Besucher verwenden ein Opt-out-Cookie, das von einem Marketer auf einer Website bereitgestellt wird

Oder der Marketer kann Benutzer verfolgen, aber eine anonymisierte IP verwenden.

Diese Methoden können sich auf den Wert und die Funktionalität von Marketo in bestimmten Bereichen auswirken. Wenn der Marketer jedoch _nichts_ der Konfiguration von Marketo ändert, bleibt die Marketo-Funktionalität unverändert.

## Browser-Einstellungen für „Nicht verfolgen“ {#browser-settings-for-do-not-track}

Web-Besuchende können ihren Browser so einstellen, dass das Tracking durch eine Website verhindert wird, indem sie „Nicht verfolgen“ (DNT) wählen. Dadurch wird das Tracking für diesen speziellen Browser und dieses Gerät verhindert. Ausführliche Informationen finden Sie in den Datenschutzeinstellungen des Browsers.

In [!DNL Munchkin] kann ein Marketing-Experte [entscheiden, ob die DNT-Einstellung des Browsers unterstützt oder ignoriert werden soll](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

In Web Personalization kann ein Marketing-Experte entscheiden, ob [die DNT-Einstellung des Browsers unterstützen oder ignorieren](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Opt-out von einer bestimmten Website {#opt-out-from-a-specific-website}

Sie können Besuchenden von Websites auch erlauben, das Website-Tracking auf Ihrer Website abzuwählen, unabhängig davon, ob die Einstellungen **Browser Do Not Tracking** konfiguriert sind oder nicht. Auf diese Weise kann der Site-Besucher seine Tracking-Voreinstellungen direkt auf Ihrer Website angeben.

Dazu müssen Sie einen -Parameter zu einem Ausschluss-Link auf einer Web-Seite hinzufügen, auf der das Tracking von [!DNL Munchkin] aktiviert ist. Dabei kann es sich um eine beliebige Web-Seite handeln, aber der Web-Seiten-Link muss den folgenden Parameter enthalten:

?marketo_opt_out=true

Nachfolgend finden Sie Beispiele für eine Web-Seite mit einem Ausschluss-Link und einer Landingpage für , nachdem auf den Link geklickt wurde. Ihre wird variieren.

Hier ist eine Webseite mit einer Schaltfläche mit dem Parameter &quot;?marketo_opt_out=true“ im Ausschluss-Link.

![](assets/understanding-privacy-settings-1.png)

Sie können eine Landingpage als Folgeseite für erstellen und veröffentlichen, wenn auf Ihren Link mit dem Parameter &quot;?marketo_opt_out=true“ geklickt wird.

![](assets/understanding-privacy-settings-2.png)

Wenn auf den Link geklickt wird, fügt Marketo dem Browser des Besuchers ein Cookie mit dem Namen **mkto_opt** hinzu, das [!DNL Munchkin] Tracking für den Site-Besucher deaktiviert, der auf den Link mit dem obigen Parameter klickt.

Um zu überprüfen, ob das Cookie platziert werden kann, stellen Sie sicher, dass Sie ein Cookie-Lead sind, und klicken Sie auf den Link. Überprüfen Sie dann Ihre Browser-Cookies, um sicherzustellen, dass das **mkto_opt_out**-Cookie hinzugefügt wurde.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Dies funktioniert derzeit nur mit [!DNL Munchkin] Versionen 152 und höher.

## Aktivieren {#opt-in}

Marketing-Experten können Benutzer aktivieren, indem sie die Funktionen von Marketo in E-Mails, Formularen, Landingpages und anderen Methoden verwenden.

## Tracking mit anonymisierter IP {#tracking-using-an-anonymized-ip}

Marketing-Experten können die Privatsphäre schützen, indem sie Benutzer mit einer anonymisierten IP-Adresse verfolgen. Fügen Sie dazu diesen Code zum RTP oder [!DNL Munchkin] JavaScript hinzu, das in die Website eingebettet ist.

* Fügen Sie [!DNL Munchkin] einfach `{"anonymizeIP",true}` zur [init-Funktion“ ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/configuration){target="_blank"}.

* Fügen Sie für Web Personalization (RTP) Folgendes zum JavaScript hinzu:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
