---
description: Ändern der Beschränkungen für den Abruf benutzerdefinierter Objekte in [!DNL Velocity Scripting] - Marketo-Dokumenten - Produktdokumentation
title: Ändern der Beschränkungen für den Abruf benutzerdefinierter Objekte in [!DNL Velocity Scripting]
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Ändern der Abrufbeschränkungen für benutzerdefinierte Objekte in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Wenn Sie [!DNL Velocity Script] verwenden, um benutzerdefinierte Objektdaten in E-Mails anzuzeigen, kann diese Funktion für Sie geeignet sein. Standardmäßig haben Sie Zugriff auf zehn übergeordnete benutzerdefinierte Objekte über das Velocity-Skript. Wenn Sie auf weitere Informationen zugreifen müssen, lesen Sie weiter.

## [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) ist eine Sprache, die auf [!DNL Java] basiert, die für die Vorlage und Skripterstellung von HTML-Inhalten entwickelt wurden. Marketo ermöglicht die Verwendung im Kontext von E-Mails mithilfe von [Skript-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Dadurch wird unter anderem Zugriff auf Daten gewährt, die in benutzerdefinierten Objekten gespeichert sind.

Sie können auf übergeordnete und untergeordnete benutzerdefinierte Objekte verweisen, die direkt mit dem Lead oder Kontakt verbunden sind, jedoch keine benutzerdefinierten Objekte der dritten Ebene. Für jedes benutzerdefinierte Objekt sind die 10 zuletzt aktualisierten Datensätze pro Person/Kontakt zur Laufzeit verfügbar und werden von der zuletzt aktualisierten Version (bei 0) zur ältesten aktualisierten Version (bei 9) sortiert.

## So ändern Sie das Limit {#how-to-change-the-limit}

1. Navigieren Sie zum Abschnitt **[!UICONTROL Admin]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Geben Sie in [!UICONTROL  Tabelle „Benutzerdefinierte Objektabrufbeschränkungen] ein neues „Übergeordnetes [!UICONTROL -Abruflimit“ ] klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Der Wert [!UICONTROL Übergeordnetes Abruflimit] muss im Bereich von 10 bis 100 liegen. Das [!UICONTROL Limit für untergeordnete ]&quot; wird automatisch festgelegt. Dies geschieht durch Division von 1000 durch das [!UICONTROL Limit für den übergeordneten Abruf]. Wenn Sie beispielsweise das übergeordnete Limit auf 50 festlegen, wird das untergeordnete Limit zu 20 (1000 ÷ 50 = 20).

Schön! Sie können jetzt von [!DNL Velocity script] aus auf weitere benutzerdefinierte Objekte zugreifen.
