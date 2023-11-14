---
description: E-Mail-Überprüfung - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Überprüfung
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: f4d2e7acaaf1ad59d716c831c7b1a2ed340a5a24
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# E-Mail-Überprüfung {#email-verification}

Für Adobe Marketo Engage-Abonnements müssen alle Benutzer, die keine API verwenden, einschließlich Marketo Engage-Administratoren, ihre E-Mail-Adresse überprüfen.

## Warum diese Funktion eingeführt wurde {#why-this-feature-was-introduced}

Marketo Engage setzt die Einführung der E-Mail-Verifizierung zur Vorbereitung der Kundenmigration zur Adobe Business Platform fort, einschließlich der Benutzermigration zu Adobe-IDs. Diese Funktion erhöht die Sicherheit vorhandener Marketo Engage-Benutzerkonten. Um sicherzustellen, dass ein Marketo Engage-Benutzer mit der richtigen Adobe ID verknüpft ist, müssen bestehende Marketo Engage-Benutzer ihre E-Mail-Adresse überprüfen. Ein Marketo Engage-Benutzer muss über eine verifizierte E-Mail-Adresse verfügen, um in eine Adobe ID migriert zu werden. Wenn ein Marketo Engage-Benutzer seine E-Mail-Adresse nicht verifiziert, kann er nicht zu einer Adobe ID migriert werden und verliert nach Abschluss der Benutzermigration für das Abonnement den Zugriff auf ein Marketo-Abonnement.

## Einladung für Benutzer {#user-invite}

Wenn ein Administrator einen Benutzer einlädt, wird dieser automatisch überprüft, sobald er auf den Link zum Einladen klickt.

## Verification Email {#verification-email}

Benutzer erhalten die folgende E-Mail, wenn die E-Mail-Verifizierung für ein Abonnement aktiviert ist oder von einem Administrator/Benutzer ausgelöst wird:

![](assets/email-verification-1.png)

>[!NOTE]
>
>Um eine Verifizierungs-E-Mail erneut an einen nicht verifizierten Benutzer zu senden, wählen Sie einfach dessen Datensatz aus und klicken Sie auf die **[!UICONTROL Email überprüfen]** Schaltfläche.

## E-Mail-Adresse ändern {#changing-an-email-address}

Wenn die E-Mail-Adresse eines Benutzers geändert wird, wird sie nicht überprüft. Sie erhalten eine E-Mail, in der sie eine erneute Überprüfung durchführen können. Benutzer können diese E-Mail manuell erneut senden, indem sie auf **[!UICONTROL Überprüfung erneut durchführen]**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Benutzer und Rollen {#users-and-roles}

In **[!UICONTROL Admin]** > **[!UICONTROL Benutzer und Rollen]**, zeigt die Spalte E-Mail-Status den Überprüfungsstatus jedes Benutzers an.

![](assets/email-verification-4.png)

## Mehrere Benutzer-Anmelde-IDs {#multiple-user-login-ids}

Nur ein Benutzerkonto kann einer einzelnen E-Mail-Adresse zugeordnet werden. Wenn mehrere Benutzerkonten mit einer einzelnen E-Mail-Adresse verknüpft sind, muss der Konflikt von Marketo Engage behoben werden, und alle mit der E-Mail-Adresse verknüpften Benutzeranmeldungen sowie drei Lösungsoptionen werden angezeigt:

* Aktuelle E-Mail für die aktuelle Benutzer-Anmelde-ID verwenden
* Verwenden einer neuen E-Mail für die aktuelle Benutzer-Anmelde-ID
* Entscheidung bis zur nächsten Anmeldung verzögern

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>Ein Benutzerkonto muss zwar einer einzelnen Adresse zugeordnet sein, es kann jedoch über eine universelle ID für mehrere Abonnements hinweg verwendet werden.
