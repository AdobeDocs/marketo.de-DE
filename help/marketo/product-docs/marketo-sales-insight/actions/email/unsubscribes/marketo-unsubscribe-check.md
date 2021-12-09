---
description: Marketo-Abmeldeprüfung - Marketo-Dokumente - Produktdokumentation
title: Überprüfung von „Marketo abbestellen“
hide: true
hidefromtoc: true
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# Überprüfung von „Marketo abbestellen“ {#marketo-unsubscribe-check}

Die Prüfung der Marketo-Abmeldung nutzt die Verbindung Ihres Teams zu Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich vom Marketo Lead Management System abgemeldet haben. Wenn ein Vertriebsbenutzer eine E-Mail mit Marketo Sales sendet, wird ein API-Aufruf an Marketo gesendet, um zu überprüfen, ob die E-Mail-ID abgemeldet wird. Ist dies der Fall, blockieren wir den Versand der E-Mail.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Aktivieren {#turning-it-on}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Abmeldungen**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicken Sie auf **Integrationen** Registerkarte. Klicken Sie im Bereich Prüfung der Marketo-Abmeldung auf den Regler, um die Prüfung zu aktivieren.

   ![](assets/marketo-unsubscribe-check-3.png)

## Was zu wissen ist {#things-to-know}

Prüfung der Marketo-Abmeldung ...

* Zählt nicht mit Ihren API-Beschränkungen
* Erfordert die Einrichtung einer Marketo-Verbindung
* Ist eine globale Einstellung
* Blockierungen von E-Mails, die von der Webanwendung, E-Mail-Clients und Salesforce gesendet werden
