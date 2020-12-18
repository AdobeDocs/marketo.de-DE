---
unique-page-id: 18317340
description: Marketo-Abmeldeprüfung - Marketing Docs - Produktdokumentation
title: Marketo-Abmeldeprüfung
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Marketo-Abmeldeprüfung {#marketo-unsubscribe-check}

Der Marketo Unsubscribe Check nutzt die Verbindung Ihres Teams mit Marketo, um zu verhindern, dass E-Mails an Personen gesendet werden, die sich vom Marketing Management System abmelden. Wenn ein Vertriebsbenutzer eine E-Mail mit Sales Connect sendet, wird ein API-Aufruf an Marketing gesendet, um zu prüfen, ob die E-Mail-ID abgemeldet wird. Ist dies der Fall, wird die Versendung der E-Mail blockiert.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## {#turning-it-on} einschalten

1. Klicken Sie in der Webanwendung auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/one-2.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Unsubscribes**.

   ![](assets/two-3.png)

1. Klicken Sie auf **Integrationen**.

   ![](assets/three-3.png)

1. Klicken Sie im Abschnitt Markieren zum Abmelden auf den Schieberegler, um die Prüfung zu aktivieren.

   ![](assets/four-2.png)

## Was Sie wissen sollten {#things-to-know}

Marketo Abmelden Check..

* Wird nicht mit Ihren API-Beschränkungen angerechnet
* Erfordert die Einrichtung einer Marketing-Verbindung
* Ist eine globale Einstellung
* Blockiert E-Mails, die von der Webanwendung, E-Mail-Clients und Salesforce gesendet werden

