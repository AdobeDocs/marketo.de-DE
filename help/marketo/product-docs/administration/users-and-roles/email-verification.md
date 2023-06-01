---
description: E-Mail-Überprüfung - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Überprüfung
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 44cca5ebad831cc39babac87ac9ebbf53df6c795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# E-Mail-Überprüfung {#email-verification}

Für Adobe Marketo Engage-Abonnements müssen alle Benutzer, die keine API verwenden, einschließlich Marketo Engage-Administratoren, ihre E-Mail-Adresse überprüfen. Single-Sign-on (SSO)-Benutzer, denen keine Administratorrolle zugewiesen wurde oder denen eine Rolle mit der Berechtigung &quot;SSO umgehen&quot;zugewiesen wurde, lassen ihre E-Mail automatisch verifizieren, wenn ihr Abonnement mit der Funktion &quot;E-Mail-Verifizierung&quot;aktiviert ist.

## Einladung für Benutzer {#user-invite}

Wenn ein Administrator einen Benutzer einlädt, wird dieser automatisch überprüft, sobald er auf den Link zum Einladen klickt. SSO-Benutzer, denen keine Administratorrolle zugewiesen wurde, werden automatisch überprüft.

## E-Mail-Adresse ändern {#changing-an-email-address}

Wenn die E-Mail-Adresse eines Benutzers geändert wird, wird sie nicht überprüft. Sie erhalten eine E-Mail, in der sie eine erneute Überprüfung durchführen können. Benutzer können diese E-Mail manuell erneut senden, indem sie auf **Überprüfung erneut durchführen**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

## Benutzer und Rollen {#users-and-roles}

In **Admin** > **Benutzer und Rollen**, zeigt die Spalte E-Mail-Status den Überprüfungsstatus jedes Benutzers an.

![](assets/email-verification-3.png)

## Mehrere Benutzer-Anmelde-IDs {#multiple-user-login-ids}

Nur ein Benutzerkonto kann einer einzelnen E-Mail-Adresse zugeordnet werden. Wenn mehrere Benutzerkonten mit einer einzelnen E-Mail-Adresse verknüpft sind, muss Marketo Engage den Konflikt lösen und alle mit der E-Mail-Adresse verknüpften Benutzeranmeldungen sowie drei Lösungsoptionen anzeigen:<p>
`1` Aktuelle E-Mail für die aktuelle Benutzer-Anmelde-ID verwenden<p>
`2` Verwenden einer neuen E-Mail für die aktuelle Benutzer-Anmelde-ID<p>
`3` Entscheidung bis zur nächsten Anmeldung verzögern

![](assets/email-verification-4.png)

## Verification Email {#verification-email}

Eingeladene Benutzer erhalten die folgende E-Mail:

![](assets/email-verification-5.png)

>[!NOTE]
>
>Um eine Verifizierungs-E-Mail erneut an einen nicht verifizierten Benutzer zu senden, wählen Sie einfach dessen Datensatz aus und klicken Sie auf die **Email überprüfen** Schaltfläche.
