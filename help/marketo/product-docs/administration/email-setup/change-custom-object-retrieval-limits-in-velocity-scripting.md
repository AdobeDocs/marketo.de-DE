---
description: Ändern von benutzerdefinierten Objektabruffriegeln in Velocity-Skripterstellung - Marketo Docs - Produktdokumentation
title: Ändern von benutzerdefinierten Object Retrieval Limits in Velocity-Skripten
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Ändern von benutzerdefinierten Object Retrieval Limits in Velocity-Skripten {#change-custom-object-retrieval-limits-in-velocity-scripting}

Wenn Sie Velocity-Skript verwenden, um benutzerdefinierte Objektdaten in E-Mails anzuzeigen, ist diese Funktion möglicherweise für Sie vorgesehen. Standardmäßig haben Sie Zugriff auf 10 übergeordnete benutzerdefinierte Objekte von Velocity Script. Wenn Sie mehr benötigen, lesen Sie weiter.

## Was ist Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) ist eine auf Java basierende Sprache, die für die Erstellung von HTML-Inhalten für Vorlagen und Skripten entwickelt wurde. Marketo ermöglicht die Verwendung im Kontext von E-Mails durch die Verwendung von [Skript-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Dies ermöglicht unter anderem den Zugriff auf Daten, die in benutzerdefinierten Objekten gespeichert sind.

Sie können auf übergeordnete und untergeordnete benutzerdefinierte Objekte verweisen, die direkt mit dem Lead oder Kontakt, aber nicht mit benutzerdefinierten Objekten der dritten Ebene verbunden sind. Für jedes benutzerdefinierte Objekt sind die 10 zuletzt aktualisierten Datensätze pro Person/Kontakt zur Laufzeit verfügbar und werden von der letzten Aktualisierung (0) bis zur ältesten Aktualisierung (9) geordnet.

## Ändern der Beschränkung {#how-to-change-the-limit}

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicken **Email**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Geben Sie in der Tabelle &quot;Benutzerdefinierte Objektabruffristen&quot;eine neue übergeordnete Abruffinität ein und klicken Sie auf **Änderungen speichern**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Der Wert für das übergeordnete Abrufindex muss zwischen 10 und 100 liegen. Die untergeordnete Abrufgrenze wird automatisch für Sie festgelegt. Dies geschieht durch Division von 1000 durch das übergeordnete Abrufflimit. Wenn Sie beispielsweise die Übergeordnete Begrenzung auf 50 festlegen, wird die Untergeordnete Beschränkung auf 20 (1000 ÷ 50 = 20) gesetzt.

Süß! Jetzt können Sie über das Velocity-Skript auf weitere benutzerdefinierte Objekte zugreifen.
