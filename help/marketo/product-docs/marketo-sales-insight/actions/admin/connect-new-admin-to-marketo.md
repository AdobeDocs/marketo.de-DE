---
description: Neue Administratoren mit Marketo verbinden - Marketo-Dokumente - Produktdokumentation
title: Neue Admin mit Marketo verbinden
hide: true
hidefromtoc: true
source-git-commit: 0ed5981470998dadd5f42384cd2e9572fec94ef6
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Neue Admin mit Marketo verbinden {#connect-new-admin-to-marketo}

Wenn der andere Administrator bereits mit Marketo verbunden ist, muss er nur Schritt 1 durchführen.

Wenn der zweite Administrator nicht mit Marketo als Administrator verbunden ist ...

1. Der primäre Administrator muss die Verbindung zwischen dem zweiten Administrator und Marketo über Einstellungen > Marketo > Benutzerzugriff trennen.

1. Sekundäre Administratoren melden sich bei ihrem MSC-Konto an, navigieren zu Einstellungen > Marketo und klicken auf **Verbinden**.

1. Jetzt ist der sekundäre Benutzer mit Marketo als Administrator verbunden.

1. Primäre Administratoren können sich jetzt anmelden und die Verbindung zu Marketo trennen.

>[!NOTE]
>
>Die anderen Benutzer bleiben verbunden, solange Benutzer B als Administrator verbunden ist, bevor Benutzer A die Verbindung trennt.

## Aktualisieren der Marketo-Verbindung {#update-your-marketo-connection}

Wenn Sie sich entscheiden, den Administrator zu entfernen, der die Marketo-Integration eingerichtet hat, lesen Sie diesen Artikel , um zu erfahren, wie Sie dies vornehmen können.

Die Marketo-Integration ist an einen Admin-Benutzer von Sales Connect/Actions gebunden. In der Regel ist dies der Administrator, der zuerst auf der Marketo-Verbindungsseite auf die Schaltfläche &quot;Verbinden&quot;geklickt und die Verbindung hergestellt hat.

Um den Administrator zu entfernen, der die Marketo-Verbindung hergestellt hat, muss zunächst eine neue Verbindung von einem anderen Administrator hergestellt werden. Wir haben die unten aufgeführten Aufgaben aufgelistet, die zu diesem Zweck durchgeführt werden müssen.

Um die Anweisungen zu vereinfachen, beziehen wir uns auf den derzeit verbundenen Administrator als Administrator A und den Administrator, mit dem Sie eine neue Verbindung zu Marketo herstellen möchten, und zwar mit Administrator B:

1. Admin A (derzeit angeschlossener Administrator) muss den Zugriff auf die Integration mit Marketo aus Admin B (neuer Administrator) entfernen.

1. Bitten Sie Admin B (neuer Administrator), eine neue Verbindung zu Marketo herzustellen.

1. Trennen Sie Admin A (ursprünglich angeschlossener Administrator).

>[!NOTE]
>
>Der ursprüngliche Administrator, der für die Marketo-Integration zuständig ist, sieht die Option &quot;Verbindung trennen&quot;, die angeklickt werden kann, wenn er zur Marketo-Integrationsseite navigiert. Andere Administratoren (die keine Verbindung hergestellt haben) werden dies nicht tun. Außerdem können Administratoren, denen Zugriff auf die Marketo-Integration gewährt wurde, nicht auf Verbinden klicken. Daher müssen Sie zuerst die Schritte ausführen, um den Zugriff auf die Integration zu entfernen.

**Entfernen des Marketo-Zugriffs aus Admin B**

Administrator A (Administrator, der ursprünglich für die Verbindung verantwortlich war) sollte diese Schritte ausführen.

1. Navigieren Sie zu Einstellungen.

1. Klicken **Marketo**.

1. Klicken **Benutzerzugriff**.

1. Suchen Sie nach dem Administrator, für den Sie die neue Marketo-Verbindung herstellen möchten.

1. Entfernen Sie den Zugriff.

**Einrichten einer neuen Verbindung für Admin B**

Auf diese Schritte sollte Admin B (neuer Administrator) folgen.

1. Navigieren Sie zu Einstellungen.

1. Klicken **Marketo**.

1. Klicken **Trennen**.

**Marketo-Integration für Admin A deaktivieren**

Auf diese Schritte sollte Admin A (ursprünglich angemeldeter Administrator) folgen.

1. Navigieren Sie zu Einstellungen.

1. Klicken **Marketo**.

1. Klicken **Trennen**.

Nachdem ein neuer Administrator eine Verbindung zu Marketo hergestellt und der ursprüngliche Administrator getrennt wurde, kann der ursprünglich verbundene Administrator sicher aus der Sales Connect/Actions-Instanz entfernt werden.
