---
description: Erfahren Sie mehr über die Marketo-Abmeldeprüfung, damit Verkäufer keine E-Mails an Personen senden können, die sich in Marketo abgemeldet haben.
title: Überprüfen der Abmeldung von Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 6%

---

# [!UICONTROL Marketo-Abmeldeprüfung] {#marketo-unsubscribe-check}

Die [!UICONTROL Marketo-Abmeldeprüfung] nutzt die Verbindung Ihres Teams zu Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich im Lead-Management-System von Marketo abgemeldet haben. Wenn ein Verkaufsbenutzer eine E-Mail mit [!DNL Marketo Sales] sendet, wird ein API-Aufruf an Marketo durchgeführt, um zu überprüfen, ob die E-Mail-ID abgemeldet wurde. Wenn dies der Fall ist, blockieren wir den Versand der E-Mail.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

## Einschalten {#turning-it-on}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Klicken [!UICONTROL &#x200B; unter „Admin] auf **[!UICONTROL Abmeldungen]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicken Sie auf die **[!UICONTROL Integrationen]**. Klicken Sie im Abschnitt [!UICONTROL Marketo-Abmeldeprüfung] auf den Schieberegler, um die Prüfung zu aktivieren.

   ![](assets/marketo-unsubscribe-check-3.png)

## Was Sie wissen sollten {#things-to-know}

Die Marketo-Abmelde-Prüfung…

* Zählt nicht auf die API-Limits
* Erfordert den Aufbau einer Marketo-Verbindung
* Ist eine globale Einstellung
* Blockiert E-Mails, die von der Webanwendung, von E-Mail-Clients und [!DNL Salesforce] gesendet werden
