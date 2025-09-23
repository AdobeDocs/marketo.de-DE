---
unique-page-id: 14352546
description: Verhindern der Integration einer Sekundären Gmail-Adresse mit Sales Connect - Marketo-Dokumente - Produktdokumentation
title: Verhindern der Integration einer sekundären Gmail-Adresse mit Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Verhindern der Integration einer Sekundären Gmail-Adresse mit [!DNL Sales Connect] {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Beschädigte Gmail-Integration (warum sende ich meine persönlichen Gmail-E-Mails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Der häufigste Grund für eine fehlerhafte Gmail-Verbindung ist eine versehentliche Integration in das persönliche Konto eines Benutzers. Dies kann vorkommen, wenn ein Benutzer auf „Verbinden“ klickt oder versucht, eine E-Mail von seinem persönlichen Konto aus zu senden. Dies kann sehr verlockend sein, da die Option beim Zugriff auf Ihr Gmail-Konto in derselben Instanz von [!DNL Chrome]wie Ihre geschäftliche E-Mail-Adresse vorhanden ist.

## Warum versucht [!DNL Sales Connect] überhaupt, meine persönliche Gmail zu integrieren? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] lässt sich über eine im Browser (installierte Erweiterung) [!DNL Chrome] Gmail integrieren. Wenn die Erweiterung erkennt, dass eine Instanz von Gmail geöffnet ist, bietet sie eine Option, um sie zu integrieren. Um eine Integration mit Ihrem persönlichen Gmail-Konto zu verhindern, empfehlen wir eines von drei Dingen…

Als anderer Benutzer [!DNL Chrome]Benutzer (empfohlen)

Klicken Sie [diesen Link](https://support.google.com/chrome/answer/2364824?hl=en), um zu erfahren, wie Sie ein weiteres [!DNL Chrome]Profil“ erstellen.

**Vorteile**: Wenn Sie sich als ein anderer Benutzer anmelden, wird eine neue Instanz von [!DNL Chrome] geöffnet. Diese Instanz ist ein brandneues Fenster von [!DNL Chrome], und keine Ihrer alten Erweiterungen wird in dieser vorhanden sein. Es enthält auch Cookies, damit Sie sich nicht jedes Mal bei Ihrer Gmail anmelden müssen.

**Nachteile**: Muss zwei Fenster von &quot;[!DNL Chrome]&quot; haben.

Andere Browser verwenden

**Positiv:** Sie einen anderen Internet-Browser (IE oder Firefox) verwenden, auf dem die Erweiterung nicht installiert ist, wird dies verhindern.

**Nachteile**: Die Verwendung mehrerer Browser kann lästig sein.

Inkognito-Fenster verwenden

**Vorteile:** Ein Inkognito-Fenster ist wie das Öffnen einer nackten Version von [!DNL Chrome]. Das bedeutet, dass keine Ihrer Erweiterungen installiert sind und [!DNL Sales Connect] keine Verbindung herstellen können.

**Nachteile**: Sie müssen sich bei jedem Start Ihres Tages bei Gmail anmelden und erneut, wenn Sie versehentlich das Fenster schließen.
