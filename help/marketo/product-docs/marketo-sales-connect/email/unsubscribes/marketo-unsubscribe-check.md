---
unique-page-id: 18317340
description: Marketo-Abmeldeprüfung - Marketo-Dokumente - Produktdokumentation
title: Überprüfung von Marketo abbestellen
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# Überprüfung von Marketo abbestellen {#marketo-unsubscribe-check}

Die Marketo-Abmeldeprüfung verwendet die Verbindung Ihres Teams zu Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich im Lead-Management-System von Marketo abgemeldet haben. Wenn ein Verkaufsbenutzer eine E-Mail mit Sales Connect sendet, wird ein API-Aufruf an Marketo durchgeführt, um zu überprüfen, ob die E-Mail-ID abgemeldet wurde. Wenn dies der Fall ist, blockieren wir den Versand der E-Mail.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Einschalten {#turning-it-on}

1. Klicken Sie in der Web-Anwendung auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one-2.png)

1. Klicken Sie unter „Admin Settings“ auf **Unsubscribes**.

   ![](assets/two-3.png)

1. Klicken Sie auf **Integrationen**.

   ![](assets/three-3.png)

1. Klicken Sie im Abschnitt Marketo-Abmeldeprüfung auf den Schieberegler, um die Prüfung zu aktivieren.

   ![](assets/four-2.png)

## Was man wissen muss {#things-to-know}

Die Marketo-Abmelde-Prüfung…

* Zählt nicht auf die API-Limits
* Erfordert den Aufbau einer Marketo-Verbindung
* Ist eine globale Einstellung
* Blockiert E-Mails, die von der Webanwendung, von E-Mail-Clients und von Salesforce gesendet werden
* Protokolliert eine fehlgeschlagene E-Mail oder verhindert, dass ein Benutzer sendet, wenn er versucht, für alle Workflows zu senden (E-Mail-Plug-in senden, einzelner Versand, Verkaufskampagne senden, Mehrfachauswahl und Senden), mit Ausnahme von [Gruppen-E-Mails](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), in denen wir verhindern, dass die E-Mails im Hintergrund gesendet werden
