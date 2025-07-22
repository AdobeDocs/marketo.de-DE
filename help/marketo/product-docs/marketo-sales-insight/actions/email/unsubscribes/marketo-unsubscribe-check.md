---
description: Marketo-Abmeldeprüfung - Marketo-Dokumente - Produktdokumentation
title: Überprüfung von Marketo abbestellen
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---

# [!UICONTROL Marketo-Abmeldeprüfung] {#marketo-unsubscribe-check}

Die [!UICONTROL Marketo-Abmeldeprüfung] nutzt die Verbindung Ihres Teams zu Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich im Lead-Management-System von Marketo abgemeldet haben. Wenn ein Verkaufsbenutzer eine E-Mail mit [!DNL Marketo Sales] sendet, wird ein API-Aufruf an Marketo durchgeführt, um zu überprüfen, ob die E-Mail-ID abgemeldet wurde. Wenn dies der Fall ist, blockieren wir den Versand der E-Mail.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Einschalten {#turning-it-on}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Klicken [!UICONTROL  unter „Admin] auf **[!UICONTROL Abmeldungen]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicken Sie auf die **[!UICONTROL Integrationen]**. Klicken Sie im Abschnitt [!UICONTROL Marketo-Abmeldeprüfung] auf den Schieberegler, um die Prüfung zu aktivieren.

   ![](assets/marketo-unsubscribe-check-3.png)

## Was man wissen muss {#things-to-know}

Die Marketo-Abmelde-Prüfung…

* Zählt nicht auf die API-Limits
* Erfordert den Aufbau einer Marketo-Verbindung
* Ist eine globale Einstellung
* Blockiert E-Mails, die von der Webanwendung, von E-Mail-Clients und [!DNL Salesforce] gesendet werden
