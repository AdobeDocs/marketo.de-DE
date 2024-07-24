---
description: E-Mail-Überprüfung - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Überprüfung
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 7b64e6e9bbd282b1e27f4c9c862df07642e9a35b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# E-Mail-Überprüfung {#email-verification}

Für Adobe Marketo Engage-Abonnements müssen alle Benutzer, die keine API verwenden, einschließlich Marketo Engage-Administratoren, ihre E-Mail-Adresse überprüfen.

## Warum diese Funktion eingeführt wurde {#why-this-feature-was-introduced}

Marketo Engage setzt die Einführung der E-Mail-Verifizierung zur Vorbereitung der Kundenmigration zur Adobe Business Platform fort, einschließlich der Benutzermigration zu Adobe-IDs. Diese Funktion erhöht die Sicherheit vorhandener Marketo Engage-Benutzerkonten. Um sicherzustellen, dass ein Marketo Engage-Benutzer mit der richtigen Adobe ID verknüpft ist, müssen bestehende Marketo Engage-Benutzer ihre E-Mail-Adresse überprüfen. Ein Marketo Engage-Benutzer muss über eine verifizierte E-Mail-Adresse verfügen, um in eine Adobe ID migriert zu werden. Wenn ein Marketo Engage-Benutzer seine E-Mail-Adresse nicht verifiziert, kann er nicht zu einer Adobe ID migriert werden und verliert nach Abschluss der Benutzermigration für das Abonnement den Zugriff auf ein Marketo-Abonnement.

## Einladung für Benutzer {#user-invite}

Wenn ein Administrator einen Benutzer einlädt, wird dieser automatisch überprüft, sobald er auf den Link zum Einladen klickt.

>[!IMPORTANT]
>
>Die Ausnahme oben ist, dass in einem reinen SSO-Abonnement _Administratoren eine neue Benutzereinladung erhalten, Benutzer, die keine Administratoren sind, dies jedoch nicht._ Benutzer, die keine Administratoren sind, müssen weiterhin den E-Mail-Verifizierungsprozess durchlaufen, um die Migration ihrer Datensätze sicherzustellen. Benutzer können den E-Mail-Verifizierungslink selbst senden, indem sie auf ihr Profilsymbol klicken, zu **Mein Konto** > **Kontoeinstellungen** navigieren und auf **Überprüfung erneut senden** klicken.

![](assets/email-verification-1.png)

## Verifizierungs-E-Mail {#verification-email}

Benutzer erhalten die E-Mail unten, wenn die E-Mail-Verifizierung für ein Abonnement aktiviert ist oder von einem Administrator/Benutzer ausgelöst wird.

Für eine erfolgreiche E-Mail-Überprüfung ist eine aktive Benutzersitzung erforderlich. Der Benutzer muss sich zunächst mit seiner Identity Provider (IdP)-URL bei seinem Marketo-Abonnement anmelden. Sobald eine Sitzung eingerichtet ist, klicken sie _dann_ auf den Link **E-Mail-Adresse überprüfen** in der E-Mail.

![](assets/email-verification-2.png)

>[!TIP]
>
>Um eine Verifizierungs-E-Mail erneut an einen nicht verifizierten Benutzer zu senden, wählen Sie einfach seinen Datensatz aus und klicken Sie auf die Schaltfläche **[!UICONTROL E-Mail verifizieren]** .

## E-Mail-Adresse ändern {#changing-an-email-address}

Wenn die E-Mail-Adresse eines Benutzers geändert wird, wird sie nicht überprüft. Sie erhalten eine E-Mail, in der sie eine erneute Überprüfung durchführen können. Benutzer können diese E-Mail manuell erneut senden, indem sie auf **[!UICONTROL Überprüfung erneut senden]** klicken.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Benutzer und Rollen {#users-and-roles}

In der Spalte &quot;**[!UICONTROL Admin]** > **[!UICONTROL Benutzer und Rollen]**&quot;zeigt die Spalte &quot;E-Mail-Status&quot;den Verifizierungsstatus jedes Benutzers an.

![](assets/email-verification-5.png)

## Mehrere Benutzer-Anmelde-IDs {#multiple-user-login-ids}

Nur ein Benutzerkonto kann einer einzelnen E-Mail-Adresse zugeordnet werden. Wenn mehrere Benutzerkonten mit einer einzelnen E-Mail-Adresse verknüpft sind, muss der Konflikt von Marketo Engage behoben werden, und alle mit der E-Mail-Adresse verknüpften Benutzeranmeldungen sowie drei Lösungsoptionen werden angezeigt:

* Aktuelle E-Mail für die aktuelle Benutzer-Anmelde-ID verwenden
* Verwenden einer neuen E-Mail für die aktuelle Benutzer-Anmelde-ID
* Entscheidung bis zur nächsten Anmeldung verzögern

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Ein Benutzerkonto muss zwar einer einzelnen Adresse zugeordnet sein, es kann jedoch über eine universelle ID für mehrere Abonnements hinweg verwendet werden.
