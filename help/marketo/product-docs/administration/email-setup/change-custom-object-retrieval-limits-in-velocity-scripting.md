---
description: Ändern Sie benutzerdefinierte Objektabfragebeschränkungen in Velocity Scripting - MarketingTo Docs - Produktdokumentation
title: Ändern von benutzerdefinierten Objektabruf-Beschränkungen in Velocity Scripting
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# Benutzerdefinierte Objektabfragebeschränkungen in Velocity-Skripten ändern {#change-custom-object-retrieval-limits-in-velocity-scripting}

Wenn Sie Velocity Script verwenden, um benutzerdefinierte Objektdaten in E-Mails anzuzeigen, ist diese Funktion möglicherweise für Sie vorgesehen. Standardmäßig haben Sie Zugriff auf 10 übergeordnete benutzerdefinierte Objekte von Velocity Script. Wenn Sie mehr Zugriff benötigen, lesen Sie weiter.

## Was ist Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) ist eine auf Java basierende Sprache, die für die Erstellung und Skripterstellung von HTML-Inhalten entwickelt wurde. Marketo erlaubt die Verwendung im Kontext von E-Mails durch die Verwendung von [Skripttokens](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Dadurch erhalten Sie unter anderem Zugriff auf Daten, die in benutzerdefinierten Objekten gespeichert werden.

Sie können auf übergeordnete und untergeordnete benutzerdefinierte Objekte verweisen, die direkt mit dem Interessenten- oder Kontaktobjekt, jedoch nicht mit benutzerdefinierten Objekten der dritten Ebene verbunden sind. Für jedes benutzerdefinierte Objekt stehen die 10 zuletzt aktualisierten Datensätze pro Person/Kontakt zur Laufzeit zur Verfügung und werden von der letzten Aktualisierung (0) bis zur ältesten aktualisierten Version (9) geordnet.

## Ändern der Beschränkung {#how-to-change-the-limit}

1. Gehen Sie zum Abschnitt **Admin**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Geben Sie in der Tabelle mit den Rückrufbeschränkungen für benutzerdefinierte Objekte eine neue Übergeordnete Abrufgrenze ein und klicken Sie auf **Änderungen speichern**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Der Wert für die übergeordnete Abrufgrenze muss zwischen 10 und 100 liegen. Die Kinderabrufgrenze wird automatisch für Sie festgelegt. Dies geschieht durch Division von 1000 durch die übergeordnete Abrufgrenze. Wenn Sie beispielsweise die Übergeordnete Beschränkung auf 50 festlegen, wird die Untergeordnete Beschränkung auf 20 (1000 / 50 = 20) gesetzt.

Süß! Jetzt können Sie über das Velocity-Skript auf weitere benutzerdefinierte Objekte zugreifen.
