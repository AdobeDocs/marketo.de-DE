---
description: Neue Administratoren mit Marketo verbinden - Marketo-Dokumente - Produktdokumentation
title: Neue Admin mit Marketo verbinden
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Neue Admin mit Marketo verbinden {#connect-new-admin-to-marketo}

Wenn der andere Administrator bereits mit Marketo verbunden ist, muss er nur Schritt 1 durchführen.

Wenn der zweite Administrator nicht mit Marketo als Administrator verbunden ist ...

1. Der primäre Administrator muss die Verbindung zwischen dem zweiten Administrator und Marketo über Einstellungen > Marketo > Benutzerzugriff trennen.

1. Der sekundäre Administrator meldet sich bei seinem MSC-Konto an, navigiert zu Einstellungen > Marketo und klickt auf **Verbinden**.

1. Jetzt ist der sekundäre Benutzer mit Marketo als Administrator verbunden.

1. Der primäre Administrator kann sich jetzt anmelden und die Verbindung zu Marketo trennen.

>[!NOTE]
>
>Die anderen Benutzer bleiben verbunden, solange Benutzer B als Administrator verbunden ist, bevor Benutzer A die Verbindung trennt.

## Aktualisieren der Marketo-Verbindung {#update-your-marketo-connection}

Wenn Sie den Admin, der die Marketo-Integration eingerichtet hat, entfernen möchten, lesen Sie diesen Artikel , um zu erfahren, wie Sie dies vornehmen können.

Die Marketo-Integration ist an einen Admin-Benutzer von Sales Connect/Actions gebunden. In der Regel ist dies der Administrator, der zuerst auf der Marketo-Verbindungsseite auf die Schaltfläche &quot;Verbinden&quot;geklickt und die Verbindung hergestellt hat.

Um den Administrator zu entfernen, der die Marketo-Verbindung hergestellt hat, muss zunächst eine neue Verbindung von einem anderen Administrator hergestellt werden. Wir haben die unten aufgeführten Aufgaben aufgelistet, die zu diesem Zweck durchgeführt werden müssen.

Um die Anweisungen zu vereinfachen, beziehen wir uns auf den derzeit verbundenen Admin als Admin A und den Admin, mit dem Sie eine neue Verbindung zu Marketo herstellen möchten, und zwar mit Admin B:

1. Admin A (derzeit angeschlossener Admin) muss den Zugriff auf die Integration mit Marketo aus Admin B (neuer Admin) entfernen.

1. Bitten Sie Admin B (neuer Administrator), eine neue Verbindung zu Marketo herzustellen.

1. Trennen Sie Admin A (ursprünglich angeschlossener Administrator).

>[!NOTE]
>
>Dem ursprünglichen für die Marketo-Integration verantwortlichen Administrator wird die Option &quot;Verbindung trennen&quot;angezeigt, die beim Navigieren zur Marketo-Integrationsseite angeklickt werden kann. Andere Administratoren (die keine Verbindung hergestellt haben) werden dies nicht tun. Außerdem können Administratoren, denen Zugriff auf die Marketo-Integration gewährt wurde, nicht auf Verbinden klicken. Daher müssen Sie zuerst die Schritte ausführen, um den Zugriff auf die Integration zu entfernen.

**Entfernen des Marketo-Zugriffs von Admin B**

Administrator A (Administrator, der ursprünglich für die Verbindung verantwortlich war) sollte diese Schritte ausführen.

1. Klicken Sie in der Webanwendung auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

1. Klicken Sie auf **Marketo**.

1. Klicken Sie auf **Benutzerzugriff**.

1. Suchen Sie nach dem Administrator, für den Sie die neue Marketo-Verbindung herstellen möchten.

1. Entfernen Sie den Zugriff.

**Einrichten einer neuen Verbindung für Admin B**

Auf diese Schritte sollte Admin B (neuer Administrator) folgen.

1. Klicken Sie in der Webanwendung auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

1. Klicken Sie auf **Marketo**.

1. Klicken Sie auf **Trennen**.

**Trennen der Marketo-Integration für Admin A**

Auf diese Schritte sollte Admin A (ursprünglich angemeldeter Admin) folgen.

1. Klicken Sie in der Webanwendung auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

1. Klicken Sie auf **Marketo**.

1. Klicken Sie auf **Trennen**.

Nachdem ein neuer Administrator eine Verbindung zu Marketo hergestellt und der ursprüngliche Administrator getrennt wurde, kann der ursprünglich verbundene Administrator sicher aus der Sales Connect/Actions-Instanz entfernt werden.
