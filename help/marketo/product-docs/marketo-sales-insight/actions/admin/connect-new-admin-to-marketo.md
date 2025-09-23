---
description: Neuen Administrator mit Marketo verbinden - Marketo-Dokumente - Produktdokumentation
title: Verbinden neuer Admins mit Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Verbinden neuer Admins mit Marketo {#connect-new-admin-to-marketo}

Wenn der andere Administrator bereits mit Marketo verbunden ist, muss er nur Schritt 1 ausführen.

Wenn der zweite Administrator nicht als Administrator mit Marketo verbunden ist…

1. Der primäre Administrator muss die Verbindung des zweiten Administrators mit Marketo unter [!UICONTROL Einstellungen] > Marketo > [!UICONTROL Benutzerzugriff] trennen.

1. Der sekundäre Administrator meldet sich bei seinem MSC-Konto an, wechselt zu [!UICONTROL Einstellungen] > Marketo und klickt auf **[!UICONTROL Verbinden]**.

1. Jetzt ist der sekundäre Benutzer als Admin mit Marketo verbunden.

1. Der Hauptadministrator kann sich jetzt anmelden und von Marketo trennen.

>[!NOTE]
>
>Die anderen Benutzer bleiben verbunden, solange Benutzer B als Administrator angemeldet ist, bevor Benutzer A die Verbindung trennt.

## Aktualisieren der Marketo-Verbindung {#update-your-marketo-connection}

Wenn Sie den Administrator bzw. die Administratorin entfernen möchten, der bzw. die die Marketo-Integration eingerichtet hat, erfahren Sie mehr darüber in diesem Artikel.

Die Marketo-Integration ist an einen Admin-Benutzer für [!DNL Sales Connect]/Aktionen gebunden. In der Regel ist dies der Administrator, der zuerst auf die Schaltfläche **[!UICONTROL Verbinden]** auf der Marketo-Verbindungsseite geklickt und die Verbindung hergestellt hat.

Um den Administrator bzw. die Administratorin zu entfernen, der bzw. die die Marketo-Verbindung hergestellt hat, muss zunächst eine neue Verbindung von einem anderen Administrator bzw. einer anderen Administratorin hergestellt werden. Nachfolgend sind die Aufgaben aufgeführt, die dazu ausgeführt werden müssen.

Um die Anweisungen zu vereinfachen, bezeichnen wir den derzeit verbundenen Administrator als Admin A und den Administrator, mit dem Sie eine neue Verbindung zu Marketo herstellen möchten:

1. Admin A (derzeit angemeldeter Administrator) muss Admin B (neuer Administrator) den Zugriff auf die Integration mit Marketo entziehen.

1. Bitten Sie Admin B (neuer Admin), eine neue Verbindung zu Marketo herzustellen.

1. Trennen Sie die Verbindung zu Administrator A (ursprünglich angemeldeter Administrator).

>[!NOTE]
>
>Der ursprüngliche Administrator, der für die Marketo-Integration verantwortlich ist, sieht die Option „Verbindung trennen“, auf die geklickt werden kann, wenn zur Marketo-Integrationsseite navigiert wird. Andere Administratoren (die keine Verbindung hergestellt haben) werden dies nicht tun. Darüber hinaus können Admins, denen Zugriff auf die Marketo-Integration gewährt wurde, nicht auf Verbinden klicken. Daher müssen Sie die Schritte ausführen, um zuerst den Zugriff auf die Integration zu entfernen.

**Entfernen des Marketo-Zugriffs von Admin B**

Ein Administrator (ursprünglich für die Verbindung verantwortlich) sollte die folgenden Schritte ausführen.

1. Klicken Sie in der Web-Anwendung auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

1. Auf **Marketo**.

1. Klicken Sie **[!UICONTROL Benutzerzugriff]**.

1. Suchen Sie nach dem Administrator, für den Sie eine neue Marketo-Verbindung herstellen möchten.

1. Entfernen Sie den Zugriff.

**Neue Verbindung für Administrator B herstellen**

Auf diese Schritte sollte Admin B (neuer Admin) folgen

1. Klicken Sie in der Web-Anwendung auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

1. Auf **Marketo**.

1. Klicken Sie **[!UICONTROL Trennen]**.

**Trennen der Marketo-Integration für Admin A**

Diesen Schritten sollte ein Administrator folgen (ursprünglich angemeldeter Administrator).

1. Klicken Sie in der Web-Anwendung auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

1. Auf **Marketo**.

1. Klicken Sie **[!UICONTROL Trennen]**.

Nachdem ein neuer Administrator eine Verbindung zu Marketo hergestellt hat und der ursprüngliche Administrator getrennt wurde, kann der ursprünglich angemeldete Administrator sicher aus der [!DNL Sales Connect]/Actions-Instanz entfernt werden.
