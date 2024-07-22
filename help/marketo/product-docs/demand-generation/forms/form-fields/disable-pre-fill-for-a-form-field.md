---
unique-page-id: 2359675
description: Vorbefüllen für ein Formularfeld deaktivieren - Marketo-Dokumente - Produktdokumentation
title: Vorbefüllen für Formularfelder deaktivieren
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Vorbefüllen für Formularfelder deaktivieren {#disable-pre-fill-for-a-form-field}

Wenn ein Webbesucher bekannt ist (Cookie), füllen Marketo-Formulare standardmäßig Felder mit den zugehörigen Informationen aus. Wenn du das ausschalten willst, hier ist, wie man es macht.

>[!NOTE]
>
>**Das Vorausfüllen des Formulars** ist standardmäßig aktiviert. Die Einstellungen für das Vorausfüllen auf Landingpage-Ebene und die Einstellungen für das Vorausfüllen auf Administratorebene überspringen die Einstellung auf Formularebene:
>
>Formular > Landingpage > Admin

## Deaktivieren der Vorbefüllung {#how-to-disable-pre-fill}

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-7.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >Das Vorausfüllen des Formulars funktioniert nicht, wenn Sie ein Formular auf Ihren eigenen Seiten einbetten. Dies funktioniert nur auf Marketo-Landingpages.

1. Wählen Sie eines der Felder aus und setzen Sie **Vorab-Ausfüllen des Formulars** auf **Deaktiviert**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >Sie können das Vorausfüllen von Formularen auch auf Landingpage-Ebene oder auf Administratorebene deaktivieren.

1. Klicken Sie auf **Beenden**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Klicken Sie auf **Genehmigen und schließen**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Sensible Felder {#sensitive-fields}

Wenn Sie [ein Feld als vertraulich markieren](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md) und dadurch verhindern, dass seine Werte in Formularen vorausgefüllt werden, wird dies in der Option &quot;Vorausfüllen&quot;angezeigt.

![](assets/disable-pre-fill.png)