---
unique-page-id: 2360337
description: Erstellen und Verwenden eines verketteten Zeichenfolgenfelds (Formel) - Marketo Docs - Produktdokumentation
title: Erstellen und Verwenden eines Felds mit verketteten Zeichenfolgen (Formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 9181a599ae715e9ffcfd84d8316dfa1c094329a6
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Erstellen und Verwenden eines Felds mit verketteten Zeichenfolgen (Formel) {#create-and-use-a-concatenated-string-formula-field}

Sie können Werte aus mehreren Feldern kombinieren oder mithilfe eines Marketo Engage-Formelfelds einen bedingten Wert erstellen.

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Klicks **[!UICONTROL Feldverwaltung]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Klicks **[!UICONTROL Neues benutzerdefiniertes Feld]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Auswählen **[!UICONTROL Formel]** für die **[!UICONTROL Typ]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Geben Sie einen **[!UICONTROL Name]** Klicken Sie für Ihr Feld auf **[!UICONTROL Erstellen]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Suchen und wählen Sie Ihr Formelfeld aus und klicken Sie auf **[!UICONTROL Regeln bearbeiten]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Fügen Sie zwei Auswahlmöglichkeiten hinzu und definieren Sie sie wie im folgenden Screenshot.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Weitere Informationen [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Jetzt können Sie das Formelfeld als Token in einer E-Mail hinzufügen.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Formelfelder können in den Spalten Landingpages, E-Mails und Smart-Listen verwendet werden. E-Mails mit Formelfeldern können _not_ mit einer Batch-Kampagne gesendet werden. Bitte verwenden Sie [email script token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) in diesem Szenario.

Gute Arbeit! Jetzt haben Sie ein intelligentes Feld, das weiß, welche Anrede auf Grundlage des Geschlechts aufgenommen werden soll. Viel Spaß damit und kreativ.
