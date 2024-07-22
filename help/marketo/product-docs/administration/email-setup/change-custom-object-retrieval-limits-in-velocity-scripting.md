---
description: "Ändern von benutzerdefinierten Objektabruffristen in [!DNL Velocity Scripting]  - Marketo Docs - Produktdokumentation"
title: "Ändern von benutzerdefinierten Objektabruffristen in [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Ändern der benutzerdefinierten Objektabruffristen in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Wenn Sie [!DNL Velocity Script] verwenden, um benutzerdefinierte Objektdaten in E-Mails anzuzeigen, ist diese Funktion möglicherweise für Sie vorgesehen. Standardmäßig haben Sie Zugriff auf 10 übergeordnete benutzerdefinierte Objekte von Velocity Script. Wenn Sie mehr benötigen, lesen Sie weiter.

## Was ist [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) ist eine Sprache, die auf [!DNL Java] basiert und für die Vorlagenerstellung und Skripterstellung von HTML-Inhalten entwickelt wurde. Marketo ermöglicht die Verwendung von [Skript-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) im Kontext von E-Mails. Dies ermöglicht unter anderem den Zugriff auf Daten, die in benutzerdefinierten Objekten gespeichert sind.

Sie können auf übergeordnete und untergeordnete benutzerdefinierte Objekte verweisen, die direkt mit dem Lead oder Kontakt, aber nicht mit benutzerdefinierten Objekten der dritten Ebene verbunden sind. Für jedes benutzerdefinierte Objekt sind die 10 zuletzt aktualisierten Datensätze pro Person/Kontakt zur Laufzeit verfügbar und werden von der letzten Aktualisierung (0) bis zur ältesten Aktualisierung (9) geordnet.

## Ändern der Beschränkung {#how-to-change-the-limit}

1. Wechseln Sie zum Abschnitt **[!UICONTROL Admin]** .

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Geben Sie in der Tabelle [!UICONTROL Benutzerdefinierte Objektabruffristen] eine neue [!UICONTROL übergeordnete Abruffrist ] ein und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Der Wert [!UICONTROL Übergeordnetes Abruflimit] muss zwischen 10 und 100 liegen. Die [!UICONTROL untergeordnete Abruffrist] wird automatisch für Sie festgelegt. Dies geschieht durch Division von 1000 durch das [!UICONTROL übergeordnete Abrufflimit]. Wenn Sie beispielsweise die Übergeordnete Begrenzung auf 50 festlegen, wird die Untergeordnete Beschränkung auf 20 (1000 ÷ 50 = 20) gesetzt.

Gut! Sie können jetzt von [!DNL Velocity script] aus auf weitere benutzerdefinierte Objekte zugreifen.
