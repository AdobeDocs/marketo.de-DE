---
description: "Ändern Sie die Beschränkungen für das Abrufen benutzerdefinierter Objekte in [!DNL Velocity Scripting] - Marketo-Dokumente - Produktdokumentation"
title: "Ändern Sie die Beschränkungen für das Abrufen benutzerdefinierter Objekte in [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Ändern Sie benutzerdefinierte Objektabruffristen in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Wenn Sie [!DNL Velocity Script] um benutzerdefinierte Objektdaten in E-Mails anzuzeigen, kann diese Funktion für Sie sein. Standardmäßig haben Sie Zugriff auf 10 übergeordnete benutzerdefinierte Objekte von Velocity Script. Wenn Sie mehr benötigen, lesen Sie weiter.

## Was ist [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) ist eine Sprache, die auf [!DNL Java] entwickelt für HTML-Vorlagenerstellung und Skripterstellung. Marketo ermöglicht die Verwendung im Kontext von E-Mails durch die Verwendung von [Skript-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Dies ermöglicht unter anderem den Zugriff auf Daten, die in benutzerdefinierten Objekten gespeichert sind.

Sie können auf übergeordnete und untergeordnete benutzerdefinierte Objekte verweisen, die direkt mit dem Lead oder Kontakt, aber nicht mit benutzerdefinierten Objekten der dritten Ebene verbunden sind. Für jedes benutzerdefinierte Objekt sind die 10 zuletzt aktualisierten Datensätze pro Person/Kontakt zur Laufzeit verfügbar und werden von der letzten Aktualisierung (0) bis zur ältesten Aktualisierung (9) geordnet.

## Ändern der Beschränkung {#how-to-change-the-limit}

1. Navigieren Sie zu **[!UICONTROL Admin]** Abschnitt.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicken **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Im [!UICONTROL Benutzerdefinierte Objektabruffristen] Tabelle, geben Sie eine neue [!UICONTROL Übergeordnetes Abruffest-Limit] und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Die [!UICONTROL Übergeordnetes Abruffest-Limit] -Wert muss im Bereich von 10 bis 100 liegen. Die [!UICONTROL Untergeordnete Abrufgrenze] wird automatisch für Sie eingestellt. Dies geschieht durch Division von 1000 durch die [!UICONTROL Übergeordnetes Abruffest-Limit]. Wenn Sie beispielsweise die Übergeordnete Begrenzung auf 50 festlegen, wird die Untergeordnete Beschränkung auf 20 (1000 ÷ 50 = 20) gesetzt.

Gut! Sie können jetzt von auf weitere benutzerdefinierte Objekte zugreifen [!DNL Velocity script].
