---
description: Routing - Marketo-Dokumente - Produktdokumentation
title: Routing
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 04359fc2bb395d442bb5215118d71de59a881749
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Routing {#routing}

In Dynamic Chat gebuchte Meetings können auf zwei Arten durchgeführt werden. Runden Sie die Aktivität ab oder verwenden Sie eine benutzerdefinierte Regel.

Round robin: Sitzungen werden den Agenten nacheinander zugewiesen. Wenn Sie also fünf Agenten und Agenten haben, die drei das letzte Meeting hatten, wird Agent vier das nächste bekommen, gefolgt von Agent fünf, dann zurück zum Agenten eins.

Benutzerdefinierte Regel: Sie können bestimmte Agenten auswählen, um Sitzungen basierend auf von Ihnen ausgewählten Attributen zu erhalten.

## Erstellen einer benutzerspezifischen Regel {#create-a-custom-rule}

In diesem Beispiel senden wir alle Sitzungen aus den angeblichen Bundesstaaten CA, OR und WA an John.

1. Klicken Sie unter &quot;Konfiguration&quot;auf **Routing-Regeln**.

   ![](assets/routing-1.png)

1. Klicken Sie auf **Benutzerspezifische Regeln** Registerkarte.

   ![](assets/routing-2.png)

1. Klicks **Regel erstellen**.

   ![](assets/routing-3.png)

1. Benennen Sie Ihre Regel. Optional können Sie eine Beschreibung hinzufügen und ihre Prioritätsstufe festlegen. Klicks **Nächste**.

   ![](assets/routing-4.png)

1. Wählen Sie die gewünschten Agenten aus.

   ![](assets/routing-5.png)

1. Ziehen Sie über die gewünschten Attribute.

   ![](assets/routing-6.png)

1. Suchen und wählen Sie die gewünschten Werte aus.

   ![](assets/routing-7.png)

1. Klicken Sie bei Auswahl aller gewünschten Werte auf **Speichern**.

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
   >Sie können mehrere Konten gleichzeitig erstellen, indem Sie auf **Kontoliste hochladen** und das Hochladen einer CSV-Datei.

1. Geben Sie den Namen und die Domäne des Unternehmens ein und wählen Sie den gewünschten Agenten aus.

   ![](assets/routing-11.png)
