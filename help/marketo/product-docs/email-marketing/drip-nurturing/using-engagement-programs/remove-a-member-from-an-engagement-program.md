---
unique-page-id: 2359951
description: Entfernen eines Mitglieds aus einem Interaktionsprogramm - Marketo-Dokumente - Produktdokumentation
title: Entfernen von Mitgliedern aus einem Interaktionsprogramm
exl-id: c97f15cc-b01a-4148-a150-84901ee2567e
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 2%

---

# Entfernen von Mitgliedern aus einem Interaktionsprogramm {#remove-a-member-from-an-engagement-program}

Entschuldigung! Wie sind diese Leute dort hineingekommen? Sie können Mitglieder aus einem Interaktionsprogramm entfernen, indem Sie die **Ändern des Programmstatus** Flussschritt.

>[!TIP]
>
>Verwenden Sie dies nicht, um Inhalte für eine Person anzuhalten. Dadurch wird die gesamte Attribution in Analytics eliminiert. Erfahren Sie mehr darüber, wie Sie [Anhalten von Personen in einem Interaktionsprogramm](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).

## Flow-Schritt {#flow-step}

1. Ziehen Sie die **Ändern des Programmstatus** Flussschritt.

   ![](assets/image2014-9-15-18-3a15-3a57.png)

   Wählen Sie den Status aus, **Nicht im Programm**.

   ![](assets/image2014-9-15-18-3a16-3a2.png)

   Groovy. Alle Mitglieder, die Sie in der Variablen [Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) wird nicht mehr in diesem Interaktionsprogramm enthalten sein.

## Personen anhalten  {#pause-people}

Manchmal möchten Sie Personen einfach in einem Interaktionsprogramm anhalten und nicht entfernen. Dies geschieht mit dem **Ändern der Interaktionsprogrammkadenz**.

>[!MORELIKETHIS]
>
>[Anhalten von Personen im Rahmen eines Interaktionsprogramms](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)
