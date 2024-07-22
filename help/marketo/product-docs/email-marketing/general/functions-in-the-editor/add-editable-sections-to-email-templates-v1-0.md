---
unique-page-id: 1900585
description: Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0 - Marketo Docs - Produktdokumentation
title: Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0 {#add-editable-sections-to-email-templates-v1.0}

Wenn Sie eine Vorlage in Version 1.0 des E-Mail-Vorlageneditors erstellen, können Sie jeden Abschnitt bearbeitbar machen, indem Sie eine spezielle &quot;`<div>`&quot;-Einstellung dafür festlegen.

>[!NOTE]
>
>**Beispiel**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regeln:

1. Die HTML muss immer gültig sein.
1. Die Klasse von **mktEditable** muss enthalten sein.
1. Die ID muss in dieser HTML eindeutig sein.
1. Keine Leerzeichen in der ID.

>[!CAUTION]
>
>mktEditable -Anweisungen können nicht verschachtelt werden.

Wenn Sie erfahren möchten, wie Sie dies im E-Mail-Vorlageneditor v2.0 durchführen, sehen Sie sich die [Syntax der E-Mail-Vorlage](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md) an.
