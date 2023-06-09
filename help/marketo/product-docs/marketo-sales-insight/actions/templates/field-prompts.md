---
description: Feldaufforderungen - Marketo-Dokumente - Produktdokumentation
title: Feldaufforderungen
source-git-commit: 7c168abc79e88c9d90786c4d5b86acbc8e0423b6
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Feldaufforderungen {#field-prompts}

Mithilfe von Feldaufforderungen können Sie E-Mails eine Textzeichenfolge hinzufügen, die entfernt oder ersetzt werden müssen, bevor die E-Mail gesendet werden kann. Auf diese Weise können Sie Benutzer daran erinnern, zusätzliche Personalisierung hinzuzufügen.

Um eine Feldaufforderung hinzuzufügen, geben Sie den gewünschten Text ein. Stellen Sie ihm ein Ausrufezeichen vor und umschließen Sie es mit geschweiften Klammern (siehe unten).

**Beispiele:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Benutzer müssen diesen Text durch eine eigene Personalisierung ersetzen, bevor die E-Mail gesendet werden kann.

![](assets/field-prompts-1.png)

>[!NOTE]
>
>Bei der Verwendung von Eingabeaufforderungen mit Verkaufskampagnen ist es am besten, diese mit manuellen E-Mail-Schritten zu verwenden. Mit diesen Schritten wird einem Benutzer eine Erinnerungsaufgabe zugewiesen, um die E-Mail zu senden, sodass er die Eingabeaufforderungen durch benutzerdefinierten Text ersetzen kann. Automatische E-Mail-Schritte in Verkaufskampagnen versuchen, automatisch zu senden, ohne dass der Benutzer die Eingabeaufforderungen ersetzen kann. Nicht ersetzte Aufforderungen führen dazu, dass die E-Mails nicht gesendet werden.
