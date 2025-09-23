---
unique-page-id: 2360337
description: Erstellen und Verwenden eines verketteten Zeichenfolgenfelds (Formel) - Marketo-Dokumente - Produktdokumentation
title: Erstellen und Verwenden eines verketteten Zeichenfolgenfelds (Formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 9%

---

# Erstellen und Verwenden eines verketteten Zeichenfolgenfelds (Formel) {#create-and-use-a-concatenated-string-formula-field}

Sie können Werte aus mehreren Feldern kombinieren oder mithilfe eines Marketo Engage-Formelfelds einen bedingten Wert erstellen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Klicken Sie **[!UICONTROL Feldverwaltung]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Feld]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Wählen Sie **[!UICONTROL Formel]** für den **[!UICONTROL Typ]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Geben Sie einen **[!UICONTROL Namen]** für Ihr Feld ein und klicken Sie dann auf **[!UICONTROL Erstellen]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Suchen Sie Ihr Formelfeld, wählen Sie es aus und klicken Sie auf **[!UICONTROL Regeln bearbeiten]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Fügen Sie zwei Auswahlmöglichkeiten hinzu und definieren Sie sie wie den folgenden Screenshot.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Weitere Informationen zu [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Jetzt können Sie das Formelfeld als Token in einer E-Mail hinzufügen.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Formelfelder können in Landingpages, E-Mails und Smart-Listen-Spalten verwendet werden. E-Mails mit Formelfeldern können _nicht_ mithilfe einer Batch-Kampagne gesendet werden. Verwenden Sie in [ Szenario ein ](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)E-Mail-Skript-Token“.

Gute Arbeit! Jetzt haben Sie ein intelligentes Feld, das weiß, welche Anrede basierend auf dem Geschlecht enthalten sein soll. Viel Spaß damit und kreativ werden.
