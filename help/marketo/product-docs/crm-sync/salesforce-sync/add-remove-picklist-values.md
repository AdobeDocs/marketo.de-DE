---
unique-page-id: 4719312
description: Auswahllistenwerte hinzufügen/entfernen - Marketo-Dokumente - Produktdokumentation
title: Auswahllistenwerte hinzufügen/entfernen
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Auswahllistenwerte hinzufügen/entfernen {#add-remove-picklist-values}

Im Folgenden finden Sie einige Informationen zum Hinzufügen und Entfernen von Werten auf der Auswahlliste in Salesforce.

## Auswahllistenwerte hinzufügen {#adding-picklist-values}

1. Wenn in Salesforce ein zusätzlicher Wert zu einem Auswahllistenfeldtyp hinzugefügt wird, erhalten Sie eine [Benachrichtigung](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} mit Angabe der Formulare, auf die sich dies auswirkt.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Wechseln Sie zum Formulareditor und [fügen Sie den zusätzlichen Wert](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} zu Ihrer Liste mit Vorschlägen hinzu.

## Auswahllistenwerte entfernen {#remove-picklist-values}

Wenn ein Wert der Auswahlliste aus einem Feld in Salesforce entfernt wird, müssen Sie diesen Wert manuell aus allen Formularen entfernen, in denen dieses Feld gehostet wird.

>[!NOTE]
>
>Wenn ein Lead- und ein Kontaktfeld in Salesforce unterschiedliche Werte aufweisen, stehen die gemeinsamen Werte zum Marketo Engage zur Verfügung.

Wenn ein Lead- und ein Kontaktfeld in Salesforce unterschiedliche Werte aufweisen:

1. Wenn Sie einer Auswahlliste einen zusätzlichen Wert in SFDC hinzufügen, erhalten Sie eine Benachrichtigung.
1. Die Benachrichtigung zeigt Ihnen, wo es verwendet wird. Sie können diesen neuen Wert jetzt bei Bedarf als Option im Formular hinzufügen.

Wenn eine Auswahlliste eines SFDC-Leads andere Werte aufweist als eine Auswahlliste für einen SFDC-Kontakt, werden die gemeinsamen Werte als Standardwertoptionen im Formular verwendet.

Wenn Sie einen Wert aus einer Auswahlliste entfernen, müssen Sie ihn manuell als Option aus Ihren Formularen entfernen.
