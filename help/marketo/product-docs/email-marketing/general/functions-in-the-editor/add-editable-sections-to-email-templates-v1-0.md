---
unique-page-id: 1900585
description: hinzufügen bearbeitbare Abschnitte zu E-Mail-Vorlagen v1.0 - Marketing-Dokumente - Produktdokumentation
title: hinzufügen bearbeitbare Abschnitte in E-Mail-Vorlagen v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# hinzufügen bearbeitbare Abschnitte in E-Mail-Vorlagen v1.0 {#add-editable-sections-to-email-templates-v1.0}

Wenn Sie eine Vorlage im E-Mail-Vorlageneditor Version 1.0 erstellen, können Sie jeden Abschnitt bearbeitbar machen, indem Sie ein spezielles `<div>` einfügen.

>[!NOTE]
>
>**Beispiel**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regeln:

1. Der HTML-Code muss immer gültig sein.
1. Die Klasse von **mktEditable** muss einbezogen werden.
1. Die ID muss in diesem HTML eindeutig sein.
1. Keine Leerzeichen in der ID.

>[!CAUTION]
>
>mktEditable-Anweisungen können nicht verschachtelt werden.

Wenn Sie wissen möchten, wie dies im E-Mail-Vorlagen-Editor v2.0 zu tun ist, lesen Sie [E-Mail-Vorlagensyntax](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md) nach.
