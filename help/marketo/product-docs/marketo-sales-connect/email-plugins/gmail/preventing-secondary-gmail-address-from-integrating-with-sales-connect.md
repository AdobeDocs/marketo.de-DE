---
unique-page-id: 14352546
description: Verhindern der Integration Sekundärer Gmail-Adressen in Sales Connect - Marketo Docs - Produktdokumentation
title: Verhindern der Integration Sekundärer Gmail-Adressen in Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Verhindern der Integration Sekundärer Gmail-Adressen in Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Fehlerhafte Gmail-Integration (warum versendet meine persönlichen Gmail-E-Mails? {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Der häufigste Grund für eine fehlerhafte Gmail-Verbindung ist die versehentliche Integration in das persönliche Konto eines Benutzers. Dies kann vorkommen, wenn ein Benutzer auf &quot;Verbinden&quot;klickt oder versucht, eine E-Mail von seinem persönlichen Konto aus zu senden. Dies kann sehr verlockend sein, da die Option beim Zugriff auf Ihr Gmail-Konto in derselben Instanz von Chrome wie Ihre Arbeits-E-Mail vorhanden sein wird.

## Warum versucht Sales Connect überhaupt, sich in meine persönliche Gmail zu integrieren? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect kann über eine im Chrome-Browser installierte Erweiterung mit Gmail integriert werden. Wenn die Erweiterung eine Gmail-Instanz öffnet, bietet sie eine Option zur Integration mit ihr. Um eine Integration mit Ihrem persönlichen Gmail-Konto zu verhindern, empfehlen wir Ihnen eine von drei Dingen...

Als anderer Chrome-Benutzer anmelden (empfohlen)

Klicken Sie auf [diesen Link](https://support.google.com/chrome/answer/2364824?hl=en) , um zu erfahren, wie Sie ein weiteres Chrome-Profil erstellen.

**Vorteile**: Wenn Sie sich als ein anderer Benutzer anmelden, wird eine neue Instanz von Chrome geöffnet. Diese Instanz ist ein ganz neues Fenster von Chrome, und in dieser wird keine Ihrer alten Erweiterungen vorhanden sein. Außerdem werden Cookies gespeichert, sodass Sie sich nicht jedes Mal bei Ihrer Gmail anmelden müssen.

**Nachteile**: Muss zwei offene Fenster von Chrome haben.

Andere Browser verwenden

**Vorteile:** Die Verwendung eines anderen Internetbrowsers (IE oder Firefox), in dem die Erweiterung nicht installiert ist, verhindert dies.

**Nachteile**: Die Verwendung mehrerer Browser kann störend sein.

Inkognito-Fenster verwenden

**Vorteile:** Ein Inkognito-Fenster gleicht dem Öffnen einer nackten Version von Chrome. Das bedeutet, dass keine Ihrer Erweiterungen installiert ist und Sales Connect nicht zum Verbinden verfügbar ist.

**Nachteile**: Sie müssen sich jedes Mal, wenn Sie Ihren Tag beginnen, bei Gmail anmelden und erneut, wenn Sie das Fenster versehentlich schließen.
