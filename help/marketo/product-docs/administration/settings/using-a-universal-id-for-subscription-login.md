---
unique-page-id: 10100311
description: Verwenden einer universellen ID für die Abonnement-Anmeldung - Marketo Docs - Produktdokumentation
title: Verwenden einer universellen ID für die Abonnement-Anmeldung
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# Verwenden einer universellen ID für die Abonnement-Anmeldung {#using-a-universal-id-for-subscription-login}

Mit einer universellen ID können Sie mit einer einzigen Anmeldung auf mehrere Marketo-Abonnement zugreifen und schnell zwischen Abonnements wechseln. Sie können jedoch auch andere Anmeldedaten für Ihre Abonnement verwenden, wenn Sie möchten.

Mit der universellen ID erstellen Sie weiterhin Support-Tickets für jedes Ihrer Abonnement.

Die Einstellungen auf Abonnement-Ebene werden für Benutzer berücksichtigt, die eine universelle ID verwenden, z. B. Rollen-, Berechtigungen- und Kennwortrichtlinien. Änderungen auf Benutzerebene werden in allen Abonnements angezeigt, z. B. Vorname, Nachname und E-Mail-Adresse.

## Einrichten einer universellen ID {#setting-up-a-universal-id}

Ihr Marketo-Administrator muss Sie von jeder einzelnen Instanz zu jedem Ihrer verschiedenen Abonnement mit derselben Anmeldung einladen. Marketo kann Ihre vorhandenen Anmeldungen nicht automatisch zusammenführen. Sobald Sie die universelle ID aktiviert haben, ist **Ihre Marketo-Instanz bis zu 30 Minuten lang nicht mehr verfügbar.** Wenn Sie eine größere Benutzerbasis haben, kann es etwas länger dauern.

>[!CAUTION]
>
>Wenn für einen Benutzer die Option &quot;Einzel-ID&quot;oder &quot;Universelle ID&quot;aktiviert ist, können deren Rollen und Arbeitsbereiche nach der Ersteinrichtung bearbeitet werden.****

>[!NOTE]
>
>Wenn Sie über mehrere Abonnement-Anmelde-IDs verfügen, können Sie auch über mehrere Community-Profil verfügen. Achten Sie darauf, die ID für Ihre universelle ID zu wählen, die mit dem Profil verbunden ist, das Sie verwenden möchten, und zwar für Ihre Produktionsinstanz, nicht für Ihre Sandbox.

## Anmelden {#logging-in}

Wenn Sie sich anmelden, um eine Einladung zu einem zweiten Abonnement mit einer universellen ID anzunehmen, wird die Anmeldeseite angezeigt. Hier müssen Sie ein Kontrollkästchen aktivieren, um die Geschäftsbedingungen zu akzeptieren. Nach der Annahme sehen Sie die normale Reset-Seite, nicht diese, für alle nachfolgenden Anmeldungen. Indem Sie die Geschäftsbedingungen akzeptieren, ermöglichen Sie Marketo, Ihre grundlegenden Profil-Daten (z. B. Vorname, Nachname und E-Mail-Adresse) an die Rechenzentren an verschiedenen Orten zu verteilen, an denen Ihr Abonnement gehostet wird.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>IDs, die Sie nicht mehr verwenden, bleiben bestehen, es sei denn, der Abonnement-Administrator löscht sie. Es wird empfohlen, diese Berichte beizubehalten, falls Ihnen beispielsweise ein eigener Bericht zugewiesen ist, auf den nur mit dieser ID zugegriffen werden kann. In diesem Fall ist es sinnvoll, diese privaten Berichte in Ihre neue universelle ID zu verschieben und dann Ihre vorhandene ID zu löschen.

## Kennwörter {#passwords}

Mit der universellen ID für mehrere Abonnement erzwingt Marketo automatisch die strengste Kennwortrichtlinie. Wenn beispielsweise einige Abonnements eine Mindestpasswortlänge erfordern und andere nicht, wird die Mindestlänge für alle Abonnement erzwungen.

Mit einer universellen ID für mehrere Abonnement können Sie nur das Kennwort ändern.

>[!NOTE]
>
>Marketo fordert Benutzer, die eine universelle ID verwenden möchten, auf, ihr Kennwort zurückzusetzen, wenn das Kennwort des aktuellen Abonnements nicht der Kennwortrichtlinie des zweiten Abonnements entspricht, zu dem sie eingeladen werden.

## Wechseln zwischen Abonnements {#switching-between-subscriptions}

Mit einer universellen ID können Sie das Abonnement sehen, bei dem Sie angemeldet sind, und andere Abonnement auswählen, auf die Sie Zugriff haben. In den meisten Fällen können Sie zwischen ihnen wechseln, ohne sich abmelden und wieder einloggen zu müssen.

![](assets/image2016-11-3-15-3a10-3a16.png)

Wenn Sie sich ab- und wieder anmelden, meldet Marketo Sie automatisch in dem Abonnement an, bei dem Sie zuletzt angemeldet waren. Sie können dann bei Bedarf zu einem anderen Abonnement wechseln.

## Community-Profile {#community-profiles}

Wenn Sie mehrere Abonnements haben, haben Sie möglicherweise mehrere Community-Profile. Es wird empfohlen, die Anmeldung auszuwählen, die mit Ihrem aktivsten Community-Profil verknüpft ist.

## Mobile Plattform {#mobile-platform}

Benutzer mit universeller ID können ihre Daten über Marketo Moments und die iPad-Ereignis-Checkin-Anwendung aus dem Abonnement anzeigen, bei dem sie sich zuletzt angemeldet haben. Sie können Abonnement nicht von der Mobile-Plattform selbst ändern.

>[!MORELIKETHIS]
>
>* [hinzufügen Einmal-Anmeldung bei einem Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Benutzeranmeldung auf SSO beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

