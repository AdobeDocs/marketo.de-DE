---
description: Erfahren Sie mehr über Feldaufforderungen in E-Mail-Vorlagen. Fügen Sie Platzhalter hinzu, die den Absender auffordern, beim Senden benutzerdefinierte Inhalte auszufüllen.
title: Eingabeaufforderungen für Felder
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
TQID: https://experienceleague.adobe.com/ahVbX8SGxaVUjSPsU-1uVc36ecIW60lwYXxDZSxC0kU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 2%

---

# Eingabeaufforderungen für Felder {#field-prompts}

Mit Eingabeaufforderungen im Feld können Sie eine Textzeichenfolge zu E-Mails hinzufügen, die entfernt oder ersetzt werden müssen, bevor die E-Mail gesendet werden kann. Dies ist eine hervorragende Möglichkeit, Benutzer daran zu erinnern, zusätzliche Personalisierungen hinzuzufügen.

Um eine Eingabeaufforderung hinzuzufügen, geben Sie den gewünschten Text ein. Stellen Sie ein Ausrufezeichen voran und schließen Sie es an geschweifte Klammern an (siehe unten).

**Beispiele:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Benutzer müssen diesen Text durch ihre eigene Personalisierung ersetzen, bevor die E-Mail gesendet werden kann.

![](assets/field-prompts-1.png)

>[!NOTE]
>
>Wenn Sie Eingabeaufforderungen mit Verkaufskampagnen verwenden, ist es am besten, sie mit manuellen E-Mail-Schritten zu verwenden. Mit diesen Schritten wird einem Benutzer eine Erinnerungsaufgabe zum Senden der E-Mail zugewiesen, sodass er die Eingabeaufforderungen durch benutzerdefinierten Text ersetzen kann. Automatische E-Mail-Schritte in Verkaufskampagnen versuchen automatisch zu senden, ohne dass der Benutzer die Eingabeaufforderungen ersetzen kann. Eingabeaufforderungen, die nicht ersetzt werden, führen dazu, dass die E-Mails nicht gesendet werden.
