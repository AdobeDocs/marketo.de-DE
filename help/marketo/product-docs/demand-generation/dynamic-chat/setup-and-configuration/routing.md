---
description: Routing - Marketo-Dokumente - Produktdokumentation
title: Routing
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Routing {#routing}

In Dynamic Chat gebuchte Meetings können auf zwei Arten durchgeführt werden. Runden Sie die Aktivität ab oder verwenden Sie eine benutzerdefinierte Regel.

Round robin: Sitzungen werden den Agenten nacheinander zugewiesen. Wenn Sie also fünf Agenten und Agenten haben, die drei das letzte Meeting hatten, wird Agent vier das nächste bekommen, gefolgt von Agent fünf, dann zurück zum Agenten eins.

Benutzerdefinierte Regel: Sie können bestimmte Agenten auswählen, um Sitzungen basierend auf von Ihnen ausgewählten Attributen zu erhalten.

>[!NOTE]
>
>Die Kontoweiterleitung hat die höchste Priorität. Wenn ein Besucher den Punkt in der Konversation erreicht, an dem er entweder ein Meeting bucht oder einen Live-Chat initiiert, wird zuerst die [Konto-Routing](#account-routing) überprüft, bevor andere Routing-Optionen in Betracht gezogen werden.

## Erstellen einer benutzerspezifischen Regel {#create-a-custom-rule}

In diesem Beispiel senden wir alle Sitzungen aus den angeblichen Bundesstaaten CA, OR und WA an John.

1. Klicken Sie unter &quot;Konfiguration&quot;auf **Routing-Regeln**.

   ![](assets/routing-1.png)

1. Klicken Sie auf die Registerkarte **Benutzerspezifische Regeln**.

   ![](assets/routing-2.png)

1. Klicken Sie auf **Regel erstellen**.

   ![](assets/routing-3.png)

1. Benennen Sie Ihre Regel. Optional können Sie eine Beschreibung hinzufügen und ihre Prioritätsstufe festlegen. Klicken Sie auf **Weiter**.

   ![](assets/routing-4.png)

1. Wählen Sie die gewünschten Agenten aus.

   ![](assets/routing-5.png)

1. Ziehen Sie über die gewünschten Attribute.

   ![](assets/routing-6.png)

1. Suchen und wählen Sie die gewünschten Werte aus.

   ![](assets/routing-7.png)

1. Wenn Sie alle gewünschten Werte ausgewählt haben, klicken Sie auf **Speichern**.

   ![](assets/routing-8.png)

## Konto-Routing {#account-routing}

Identifizieren und laden Sie Ihr Zielkonto und die entsprechenden Vertriebseigentümer hoch und leiten Sie Besucher, die von diesen Konten kommen, direkt zum entsprechenden Kontoinhaber weiter.

![](assets/routing-9.png)

### Hinzufügen eines Kontos {#add-an-account}

In diesem Beispiel leiten wir alle Mitarbeiter von Lego direkt zum Agenten Steven weiter.

1. Klicken Sie auf der Registerkarte Konto-Routing auf **+ Konto hinzufügen**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >Sie können mehrere Konten gleichzeitig erstellen, indem Sie auf **Kontoliste hochladen** klicken und eine CSV-Datei hochladen.

1. Geben Sie den Namen und die Domäne des Unternehmens ein und wählen Sie den gewünschten Agenten aus.

   ![](assets/routing-11.png)
