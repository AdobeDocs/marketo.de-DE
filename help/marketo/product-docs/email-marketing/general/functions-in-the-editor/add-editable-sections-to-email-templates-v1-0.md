---
unique-page-id: 1900585
description: Erfahren Sie, wie Sie in Version 1.0 bearbeitbare Abschnitte zu E-Mail-Vorlagen hinzufügen. Benutzerinnen und Benutzer können bestimmte Bereiche bearbeiten, während der Rest gesperrt bleibt.
title: Hinzufügen bearbeitbarer Abschnitte zu E-Mail-Vorlagen v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
TQID: https://experienceleague.adobe.com/j2rwpy7Bq-HH3-mva5FkDb3kKH8cvlH2hMUp0ic7sno
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 14%

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
