---
description: Routing - Marketo-Dokumente - Produktdokumentation
title: Routing
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 1%

---

# Routing {#routing}

In Dynamic Chat gebuchte Meetings können auf zwei Arten weitergeleitet werden. Round Robin oder unter Verwendung einer benutzerdefinierten Regel.

Round Robin: Meetings werden Agenten sequenziell zugewiesen. Wenn Sie also fünf Agenten haben, und Agent drei hat das letzte Meeting genommen, dann bekommt Agent vier den nächsten, gefolgt von Agent fünf, dann zurück zu Agent eins.

Benutzerdefinierte Regel: Sie können bestimmte Agenten auswählen, die basierend auf ausgewählten Attributen Meetings empfangen sollen.

>[!NOTE]
>
>Das Konto-Routing hat die höchste Priorität. Wenn ein Besucher den Punkt im Gespräch erreicht, um entweder ein Meeting zu buchen oder einen Live-Chat zu initiieren[ wird ](#account-routing)Konto-Routing“ zuerst überprüft, bevor andere Routing-Optionen berücksichtigt werden.

## Erstellen einer benutzerdefinierten Regel {#create-a-custom-rule}

In diesem Beispiel senden wir alle Besprechungen aus den abgeleiteten Zuständen von CA, OR und WA an Agent John.

1. Klicken Sie unter Konfiguration auf **Routing-Regeln**.

   ![](assets/routing-1.png)

1. Klicken Sie auf **Registerkarte** Benutzerdefinierte Regeln“.

   ![](assets/routing-2.png)

1. Klicken Sie **Regel erstellen**.

   ![](assets/routing-3.png)

1. Benennen Sie Ihre Regel. Optional können Sie eine Beschreibung hinzufügen und deren Prioritätsstufe festlegen. Klicken Sie auf **Weiter**.

   ![](assets/routing-4.png)

1. Wählen Sie Ihren gewünschten Agenten aus.

   ![](assets/routing-5.png)

1. Ziehen Sie das/die gewünschte(n) Attribut(e).

   ![](assets/routing-6.png)

1. Suchen Sie die gewünschten Werte und wählen Sie sie aus.

   ![](assets/routing-7.png)

1. Wenn Sie alle gewünschten Werte ausgewählt haben, klicken Sie auf **Speichern**.

   ![](assets/routing-8.png)

## Konto-Routing {#account-routing}

Identifizieren und hochladen Ihres Zielkontos und der jeweiligen Vertriebsinhaber und leiten Sie Besucher, die aus diesen Konten kommen, direkt an den jeweiligen Kontoinhaber weiter.

![](assets/routing-9.png)

### Konto hinzufügen {#add-an-account}

In diesem Beispiel leiten wir alle Mitarbeiter von Lego direkt zu Agent Steven weiter.

1. Klicken Sie auf der Registerkarte Konto-Routing auf **+ Konto hinzufügen**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >Sie können mehrere Konten gleichzeitig erstellen, indem Sie auf **Kontoliste hochladen** und eine CSV-Datei hochladen.

1. Geben Sie den Namen und die Domain des Unternehmens ein und wählen Sie den gewünschten Agenten aus.

   ![](assets/routing-11.png)
