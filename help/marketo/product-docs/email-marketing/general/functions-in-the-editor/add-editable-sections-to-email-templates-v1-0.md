---
unique-page-id: 1900585
description: Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0 - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 16%

---

# Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0 {#add-editable-sections-to-email-templates-v1.0}

Wenn Sie eine Vorlage im E-Mail-Vorlageneditor v1.0 erstellen, können Sie jeden Bereich bearbeiten, indem Sie ihn mit einem speziellen `<div>` versehen.

>[!NOTE]
>
>**Beispiel**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regeln:

1. Die HTML muss immer gültig sein.
1. Die Klasse **mktEditable** muss enthalten sein.
1. Die ID muss in dieser HTML eindeutig sein.
1. Keine Leerzeichen in der ID.

>[!CAUTION]
>
>mktEditable-Anweisungen können nicht verschachtelt werden.

Wenn Sie erfahren möchten, wie Sie dies im E-Mail-Vorlageneditor v2.0 tun können, lesen Sie [E-Mail-Vorlagensyntax](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
