---
description: Benachrichtigungsdetails für Marketo Engage-Benutzende, die die Benachrichtigung zum Herstellen einer WebSocket-Verbindung nicht erhalten haben
title: Benachrichtigung - WebSocket-Verbindung
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 30%

---

# Benachrichtigung: WebSocket-Verbindung {#notification-websocket-connection}

Dieses Dokument richtet sich an Marketo Engage-Benutzer, die die folgende Benachrichtigung in ihrer Marketo-Instanz erhalten haben: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Wenn Sie oder Ihr Unternehmen einschränkende Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie oder Ihre bzw. Ihr Netzwerkadmin möglicherweise bestimmte Domains und IP-Adressbereiche auf die Zulassungsliste setzen, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

Der Marketo-Support ist nicht für die Implementierung der folgenden Protokolle eingerichtet. Wenn Sie Hilfe benötigen, teilen Sie dieses Dokument bitte mit Ihrem IT-Team. Wenn der Web-Zugriff mithilfe einer -Zulassungsliste eingeschränkt wird, bitten Sie sie, die folgenden Domains (einschließlich des Sternchens) hinzuzufügen, um alle Marketo-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
