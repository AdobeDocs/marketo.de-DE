---
unique-page-id: 2360337
description: Erstellen und Verwenden eines Felds für verkettete Zeichenfolge (Formel) - Marketo Docs - Produktdokumentation
title: Erstellen und Verwenden eines verketteten Zeichenfolgenfelds (Formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Erstellen und Verwenden eines Felds für verkettete Zeichenfolge (Formel) {#create-and-use-a-concatenated-string-formula-field}

Sie können Werte aus mehreren Feldern kombinieren oder einen bedingten Wert mit einem Marketo-Formularfeld erstellen.

1. Wechseln Sie zu **Admin** und klicken Sie auf **Feldverwaltung**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Klicken Sie auf **Neues benutzerdefiniertes Feld**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Wählen Sie **Formel** für **Typ**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Geben Sie einen **Name** für Ihr Feld ein und klicken Sie dann auf **Erstellen**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Suchen Sie nach Ihrem Formelfeld und wählen Sie es aus und klicken Sie dann auf **Regeln bearbeiten**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. hinzufügen Sie zwei Auswahlmöglichkeiten und definieren Sie sie wie den Screenshot unten.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Erfahren Sie mehr über [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Jetzt können Sie das Formelfeld als Token in einer E-Mail hinzufügen.

   ![](assets/seven.png)

>[!NOTE]
>
>Formularfelder können in Landingpages, E-Mails und Spalten mit intelligenter Liste verwendet werden (sie werden nicht exportiert). E-Mails mit Formelfeldern können **nicht** mit einer Batch-Kampagne gesendet werden. Verwenden Sie in diesem Szenario ein [E-Mail-Skript-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md).

Gute Arbeit! Jetzt haben Sie ein intelligentes Feld, das weiß, welche Begrüßung auf der Grundlage des Geschlechts einzubeziehen ist. Viel Spaß damit und kreativ.
