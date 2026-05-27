---
solution: Marketo Engage
product: marketo
title: Personalisierungs-Token
description: Erfahren Sie, wie Sie Personalisierungs-Token in der E-Mail-Designer verwenden. Fügen Sie dynamische Empfängerdaten zu Ihrem E-Mail-Inhalt hinzu.
level: Beginner, Intermediate
feature: Email Designer
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
hide: true
TQID: https://experienceleague.adobe.com/2F6SP0sUvcScw0Y86X10nRTfL2b45krGTLeSi-td7Uc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 1%

---

# Personalisierungs-Token {#personalization-tokens}

E-Mail-Designer hat ein anderes Format als der klassische E-Mail-Editor, wenn es um E-Mail-Personalisierungs-Token geht. Die Änderung wurde implementiert, um die Kompatibilität mit Handlebar-Skripten zu verbessern und den E-Mail-Erstellungsprozess zu optimieren.

>[!AVAILABILITY]
>
>Ab dem 23. Mai 2025 wird diese Funktion Marketo Engage-Benutzenden in Batches bereitgestellt, wobei pro Woche eine Region aktualisiert wird. Während des Rollouts migrieren alle mit dem neuen E-Mail-Designer erstellten E-Mails vorhandene Token automatisch in das neue Format. Mit diesem Update sind alle Token nur in englischer Sprache verfügbar.

## Primärer Anwendungsfall {#primary-use-case}

Diese Verbesserung kommt in erster Linie denjenigen zugute, die von [Velocity-Skripterstellung](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting){target="_blank"} zu Handlebar-Skripterstellung wechseln. Der neue E-Mail-Designer unterstützt nur das neue Token-Format. Das aktualisierte Format beseitigt Leerzeichen und führt eine überarbeitete Standardtextstruktur ein, um ein reibungsloseres und effizienteres Skripterlebnis zu gewährleisten.

## Token-Erlebnis {#token-experience}

Ein Blick auf das Token-Erlebnis, alt und neu.

### Altes Format {#old-format}

Im klassischen E-Mail-Editor können Sie Token mit Leerzeichen wie `lead.Anonymous IP` oder `member.registration code` hinzufügen. Das Format für den Standardtext war: `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### Neues Format {#new-format}

In E-Mail-Designer müssen Sie [Binnenmajuskel-Schreibweise](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) oder Unterstriche für Token (z. B. `lead.anonymousIP` oder `member.registration_code`) verwenden. Das Format für den Standardtext ändert sich ebenfalls in `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## Zu beachtende Punkte {#things-to-note}

* Der Personalisierungseditor bietet außerdem die folgenden Funktionen zur Vereinfachung der Bearbeitung:

   * Rückgängig/Wiederholen
   * Suchen/Suchen und Ersetzen

* **Alle** Token, die zuvor in Marketo Engage unterstützt wurden, werden im neuen Personalisierungseditor unterstützt.
