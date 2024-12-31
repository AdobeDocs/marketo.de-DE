---
unique-page-id: 14352546
description: Verhindern der Integration einer Sekundären Gmail-Adresse mit Sales Connect - Marketo-Dokumente - Produktdokumentation
title: Verhindern der Integration einer Sekundären Gmail-Adresse mit Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Verhindern der Integration einer Sekundären Gmail-Adresse mit Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Beschädigte Gmail-Integration (warum sende ich meine persönlichen Gmail-E-Mails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Der häufigste Grund für eine fehlerhafte Gmail-Verbindung ist eine versehentliche Integration in das persönliche Konto eines Benutzers. Dies kann vorkommen, wenn ein Benutzer auf „Verbinden“ klickt oder versucht, eine E-Mail von seinem persönlichen Konto aus zu senden. Dies kann sehr verlockend sein, da die Option beim Zugriff auf Ihr Gmail-Konto in derselben Instanz von Chrome wie Ihre geschäftliche E-Mail vorhanden sein wird.

## Warum versucht Sales Connect überhaupt, meine persönliche Gmail-Integration zu integrieren? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect kann über eine im Chrome-Browser installierte Erweiterung mit Gmail integriert werden. Wenn die Erweiterung erkennt, dass eine Instanz von Gmail geöffnet ist, bietet sie eine Option, um sie zu integrieren. Um eine Integration mit Ihrem persönlichen Gmail-Konto zu verhindern, empfehlen wir eines von drei Dingen…

Melden Sie sich als ein anderer Chrome-Benutzer an (empfohlen)

Klicken Sie [diesen Link](https://support.google.com/chrome/answer/2364824?hl=en), um zu erfahren, wie Sie ein weiteres Chrome-Profil erstellen.

**Vorteile**: Wenn Sie sich als ein anderer Benutzer anmelden, wird eine neue Instanz von Chrome geöffnet. Diese Instanz ist ein brandneues Fenster von Chrome, und keine Ihrer alten Erweiterungen ist in dieser vorhanden. Es enthält auch Cookies, damit Sie sich nicht jedes Mal bei Ihrer Gmail anmelden müssen.

**Nachteile**: Muss zwei Fenster von Chrome geöffnet haben.

Andere Browser verwenden

**Positiv:** Sie einen anderen Internet-Browser (IE oder Firefox) verwenden, auf dem die Erweiterung nicht installiert ist, wird dies verhindern.

**Nachteile**: Die Verwendung mehrerer Browser kann lästig sein.

Inkognito-Fenster verwenden

**Positiv:** Ein Inkognito-Fenster ist wie das Öffnen einer nackten Version von Chrome. Das bedeutet, dass keine Ihrer Erweiterungen installiert ist und Sales Connect nicht zur Verbindung verfügbar ist.

**Nachteile**: Sie müssen sich bei jedem Start Ihres Tages bei Gmail anmelden und erneut, wenn Sie versehentlich das Fenster schließen.
