---
unique-page-id: 10100311
description: Verwenden einer universellen ID für die Anmeldung von Abonnements - Marketo Docs - Produktdokumentation
title: Verwendung einer universellen ID zur Anmeldung von Abonnements
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 2bd8a7c2a1fe467cc73460807faee42e39faea5d
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Verwendung einer universellen ID zur Anmeldung von Abonnements {#using-a-universal-id-for-subscription-login}

Mit einer universellen ID können Sie mit einer einzigen Anmeldung auf mehrere Marketo-Abonnements zugreifen und schnell zwischen Abonnements wechseln. Sie können jedoch bei Bedarf verschiedene Anmeldungen für Ihre Abonnements verwenden.

Mit der universellen ID erstellen Sie weiterhin Support-Tickets für jedes Ihrer individuellen Abonnements.

Einstellungen auf Abonnementebene werden für Benutzer berücksichtigt, die eine universelle ID verwenden, z. B. Rollen, Berechtigungen und Kennwortrichtlinien. Änderungen auf Benutzerprofilebene werden in allen Abonnements übernommen, z. B. Vorname, Nachname und E-Mail-Adresse.

## Einrichten einer universellen ID {#setting-up-a-universal-id}

Alle Marketo-Abonnements verfügen über die optionale Funktion Universal ID . Ihr Marketo-Administrator muss Sie von jeder Instanz aus zu jedem Ihrer Abonnements mit demselben Login einladen. Marketo kann Ihre vorhandenen Anmeldungen nicht automatisch zusammenführen.

>[!NOTE]
>
>Wenn Sie über mehrere Anmelde-IDs verfügen, können Sie auch über mehrere Community-Profile verfügen. Wählen Sie unbedingt die Kennung für Ihre universelle ID aus, die mit dem Profil verbunden ist, das Sie verwenden möchten, und zwar für Ihre Produktionsinstanz, nicht für Ihre Sandbox.

## Anmelden {#logging-in}

Wenn Sie sich anmelden, um eine Einladung zu einem zweiten Abonnement mit einer universellen ID anzunehmen, wird die Anmeldeseite für Opt-in angezeigt. Hier müssen Sie ein Kontrollkästchen aktivieren, um die Geschäftsbedingungen zu akzeptieren. Nachdem Sie akzeptiert haben, sehen Sie die normale Zurücksetzseite, nicht diese für alle nachfolgenden Anmeldungen. Durch die Annahme der Nutzungsbedingungen gestatten Sie Marketo, Ihre grundlegenden Profildaten (wie Vorname, Nachname und E-Mail-Adresse) an die Rechenzentren an verschiedenen Standorten zu verteilen, an denen Ihr Abonnement gehostet wird.

![](assets/using-a-universal-id-for-subscription-login-1.png)

>[!TIP]
>
>IDs, die Sie nicht mehr verwenden, bleiben bestehen, es sei denn, der Abonnementadministrator löscht sie. Es wird empfohlen, diese beizubehalten, falls Sie beispielsweise einen privaten Bericht haben, der sich selbst zugewiesen ist und auf den nur mit dieser ID zugegriffen werden kann. In diesem Fall ist es sinnvoll, diese privaten Berichte in Ihre neue universelle ID zu verschieben und dann Ihre vorhandene ID zu löschen.

## Passwörter {#passwords}

Mit der universellen ID für mehrere Abonnements erzwingt Marketo automatisch die strengste Kennwortrichtlinie. Wenn beispielsweise einige Abonnements eine Mindestpasswortlänge erfordern und andere nicht, wird die Mindestlänge für alle Abonnements erzwungen.

Bei einer universellen ID für mehrere Abonnements können Sie nur das Kennwort ändern.

>[!NOTE]
>
>Marketo fordert Benutzer, die die universelle ID verwenden möchten, auf, ihr Kennwort zurückzusetzen, wenn das Kennwort des aktuellen Abonnements nicht der Kennwortrichtlinie des zweiten Abonnements entspricht, für das sie eingeladen werden.

## Wechseln zwischen Abonnements {#switching-between-subscriptions}

Mit einer universellen ID können Sie das Abonnement sehen, bei dem Sie angemeldet sind, und andere Abonnements auswählen, auf die Sie Zugriff haben. In den meisten Fällen können Sie zwischen ihnen wechseln, ohne sich abmelden und wieder anmelden zu müssen.

![](assets/using-a-universal-id-for-subscription-login-2.png)

Wenn Sie sich abmelden und wieder anmelden, meldet sich Marketo automatisch bei dem Abonnement an, bei dem Sie zuletzt angemeldet waren. Sie können dann bei Bedarf zu einem anderen Abonnement wechseln.

## Community-Profile {#community-profiles}

Wenn Sie mehrere Abonnements haben, können Sie über mehrere Community-Profile verfügen. Es wird empfohlen, die Anmeldung auszuwählen, die mit Ihrem aktivsten Community-Profil verknüpft ist.

## Mobile Platform {#mobile-platform}

Benutzer mit universeller ID können ihre Daten in [Marketo-Momente](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/marketo-moments/understanding-moments/understanding-marketo-moments.md){target="_blank"} and the [event check-in application](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md){target="_blank"} aus dem Abonnement, bei dem sie sich zuletzt angemeldet haben. An der Mobile-Plattform selbst können Sie keine Abonnements ändern.

>[!MORELIKETHIS]
>
>* [Single Sign-On zu einem Portal hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md){target="_blank"}
>* [Benutzeranmeldung auf &quot;Nur SSO&quot;beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
