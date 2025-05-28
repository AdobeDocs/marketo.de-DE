---
solution: Marketo Engage
product: marketo
title: Personalization-Token
description: Erfahren Sie, wie Sie in der neuen Marketo Engage Email Designer Personalisierungs-Token verwenden.
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 0abb2a7499541b8efbf3000bcd9fc9c1a79e43e1
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Personalization-Token {#personalization-tokens}

Die E-Mail-Designer hat ein anderes Format als der klassische E-Mail-Editor, wenn es um E-Mail-Personalisierungs-Token geht. Die Änderung wurde implementiert, um die Kompatibilität mit Handlebar-Skripten zu verbessern und den E-Mail-Erstellungsprozess zu optimieren.

>[!AVAILABILITY]
>
>Ab dem 23. Mai 2025 wird diese Funktion Marketo Engage-Benutzenden in Batches bereitgestellt, wobei pro Woche eine Region aktualisiert wird. Während des Rollouts migrieren alle mit dem neuen E-Mail-Designer erstellten E-Mails vorhandene Token automatisch in das neue Format. Mit diesem Update sind alle Token nur in englischer Sprache verfügbar.

## Primärer Anwendungsfall {#primary-use-case}

Diese Verbesserung kommt in erster Linie denjenigen zugute, die von [Velocity-Skripterstellung](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting){target="_blank"} zu Handlebar-Skripterstellung wechseln. Die neue E-Mail-Designer unterstützt nur das neue Token-Format. Das aktualisierte Format beseitigt Leerzeichen und führt eine überarbeitete Standardtextstruktur ein, um ein reibungsloseres und effizienteres Skripterlebnis zu gewährleisten.

## Token-Erlebnis {#token-experience}

Ein Blick auf das Token-Erlebnis, alt und neu.

### Altes Format {#old-format}

Im klassischen E-Mail-Editor können Sie Token mit Leerzeichen wie `lead.Anonymous IP` oder `member.registration code` hinzufügen. Das Format für den Standardtext war: `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="500" zoomable="yes"}

### Neues Format {#new-format}

Im E-Mail-Designer müssen Sie sich an [Binnenmajuskel-Schreibweise](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) oder Unterstriche für Token (z. B. `lead.anonymousIP` oder `member.registration_code`) anpassen. Das Format für den Standardtext ändert sich ebenfalls in `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="600" zoomable="yes"}

## Zu beachtende Punkte {#things-to-note}

* Der Personalisierungseditor bietet außerdem die folgenden Funktionen zur Vereinfachung der Bearbeitung:

   * Rückgängig/Wiederholen
   * Suchen/Suchen und Ersetzen
   * AutoVervollständigen

* **Alle** Token, die zuvor in Marketo Engage unterstützt wurden, werden im neuen Personalisierungseditor unterstützt.
