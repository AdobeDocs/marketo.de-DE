---
description: Marketo-Abmeldeprüfung - Marketo-Dokumente - Produktdokumentation
title: Überprüfung von Marketo abbestellen
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# Überprüfung von Marketo abbestellen {#marketo-unsubscribe-check}

Die Marketo-Abmeldeprüfung verwendet die Verbindung Ihres Teams zu Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich im Lead-Management-System von Marketo abgemeldet haben. Wenn ein Verkaufsbenutzer eine E-Mail mit Marketo Sales sendet, wird ein API-Aufruf an Marketo durchgeführt, um zu überprüfen, ob die E-Mail-ID abgemeldet wurde. Wenn dies der Fall ist, blockieren wir den Versand der E-Mail.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Einschalten {#turning-it-on}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Klicken Sie unter „Admin Settings“ auf **Unsubscribes**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicken Sie auf die **Integrationen**. Klicken Sie im Abschnitt Marketo-Abmeldeprüfung auf den Schieberegler, um die Prüfung zu aktivieren.

   ![](assets/marketo-unsubscribe-check-3.png)

## Was man wissen muss {#things-to-know}

Die Marketo-Abmelde-Prüfung…

* Zählt nicht auf die API-Limits
* Erfordert den Aufbau einer Marketo-Verbindung
* Ist eine globale Einstellung
* Blockiert E-Mails, die von der Webanwendung, von E-Mail-Clients und von Salesforce gesendet werden
