---
description: Benachrichtigung - Websocket-Verbindung - Marketo-Dokumente - Produktdokumentation
title: Benachrichtigung - Websocket-Verbindung
hide: true
hidefromtoc: true
source-git-commit: 77300e8d620887b5c1d14a4f979a96488b6eec87
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Benachrichtigung: Websocket-Verbindung {#notification-websocket-connection}

Dieser Artikel richtet sich an Marketo Engage-Benutzer, die die folgende Benachrichtigung in ihrer Marketo-Instanz erhalten haben: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Wenn Sie oder Ihr Unternehmen restriktive Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie oder Ihr Netzwerkadministrator möglicherweise bestimmte Domänen und IP-Adressbereiche in Zulassungslisten eintragen, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

Der Marketo-Support ist nicht für die Implementierung der folgenden Protokolle eingerichtet. Wenn Sie Hilfe benötigen, geben Sie diesen Artikel bitte an Ihr IT-Team weiter. Wenn sie den Webzugriff mithilfe einer Zulassungsliste beschränken, bitten Sie sie, die folgenden Domänen hinzuzufügen (einschließlich des Sternchens), um alle Marketo-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
