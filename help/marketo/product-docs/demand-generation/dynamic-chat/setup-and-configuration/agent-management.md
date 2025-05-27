---
description: Agentenverwaltung - Marketo-Dokumente - Produktdokumentation
title: Agentenverwaltung
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 1%

---

# Agentenverwaltung {#agent-management}

Zeigen Sie in der Agentenverwaltung eine Liste der Agenten in Ihrer Dynamic Chat-Instanz an, verwalten Sie Teams und legen Sie Fallback-Regeln fest.

![](assets/agent-management-1.png)

## Agentinnen bzw. Agenten {#agents}

Auf dieser Registerkarte werden alle Agenten in Ihrer Dynamic Chat-Instanz aufgelistet. Sie enthält Informationen wie Namen, E-Mail-Adresse, Live-Chat-Status und mehr.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Erscheint kein Agent, den Sie _gerade_ hinzugefügt haben? Es kann bis zu zwei Stunden dauern, bis sie hier angezeigt werden, nachdem sie in der Adobe Admin Console hinzugefügt wurden.

## Teams {#teams}

Administratoren können Agententeams erstellen, um die Weiterleitung an bestimmte Gruppen von Kundendienstmitarbeitern zu erleichtern.

>[!AVAILABILITY]
>
>Der Zugriff auf Teams erfordert ein Dynamic Chat Prime-Abonnement. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

![](assets/agent-management-3.png)

### Erstellen eines Teams {#create-a-team}

1. Klicken Sie auf **+ Team erstellen**.

   ![](assets/agent-management-4.png)

1. Geben Sie Ihrem Team einen Namen.

   ![](assets/agent-management-5.png)

1. Klicken Sie auf **Agenten hinzufügen** und wählen Sie die gewünschten Agenten aus.

   ![](assets/agent-management-6.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/agent-management-7.png)

## Fallback-Regeln {#fallback-rules}

### Meeting-Fallback {#meeting-fallback}

Wählen Sie eine Standard-(System-)Nachricht aus oder schreiben Sie eine benutzerdefinierte Nachricht, die Besucher sehen können, wenn die Besprechungsbuchung nicht verfügbar ist.

![](assets/agent-management-8.png)

### Fallback zum Live-Chat {#live-chat-fallback}

Wählen Sie eine Standardnachricht (System) aus oder schreiben Sie eine benutzerdefinierte Nachricht, die Besuchenden angezeigt wird, wenn der Live-Chat nicht verfügbar ist.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Wenn Sie das Kontrollkästchen _Buchungsoption für Besprechungen einschließen_ aktivieren, hat der Chat-Besucher die Möglichkeit, ein Meeting zu buchen, wenn keine Agenten für den Live-Chat verfügbar sind.
>
>* **Für benutzerdefinierte Regeln/Teams als Live-Chat-Karte**: Wenn Agenten gesucht werden, wenn sie nicht verfügbar sind oder keine Verbindung herstellen konnten, wird auf Round Robin zurückgegriffen, um nach „Verfügbare Agenten“ zu suchen (alle, die zu diesem Zeitpunkt verfügbar sind, unabhängig davon, welche Routing-Logik/Regel im Stream platziert wurde).

>[!TIP]
>
>Beim Erstellen einer benutzerdefinierten Nachricht können Sie die Schriftart gestalten, Links verwenden oder sogar Emojis einfügen! `:)`
