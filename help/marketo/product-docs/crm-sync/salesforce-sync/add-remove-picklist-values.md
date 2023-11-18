---
unique-page-id: 4719312
description: Hinzufügen/Entfernen von Picklist-Werten - Marketo Docs - Produktdokumentation
title: Hinzufügen/Entfernen von Picklist-Werten
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Hinzufügen/Entfernen von Picklist-Werten {#add-remove-picklist-values}

Im Folgenden finden Sie einige Informationen zum Hinzufügen und Entfernen von Picklist-Werten in Salesforce.

## Hinzufügen von Picklist-Werten {#adding-picklist-values}

1. Wenn ein zusätzlicher Wert in Salesforce zu einem Picklist-Feldtyp hinzugefügt wird, erhalten Sie eine [Benachrichtigung](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} Angabe der Formulare, auf die sich dies auswirken wird.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Wechseln Sie zum Formular-Editor und [den zusätzlichen Wert hinzufügen](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} zu Ihrer Liste mit Vorschlägen.

## Entfernen von Picklist-Werten {#remove-picklist-values}

Wenn ein Auswahllistenwert aus einem Feld in Salesforce entfernt wird, müssen Sie diesen Wert manuell aus allen Formularen entfernen, die dieses Feld hosten.

>[!NOTE]
>
>Wenn ein Lead- und ein Kontaktfeld in Salesforce unterschiedliche Werte aufweisen, sind die gemeinsamen Werte für Marketo Engage verfügbar.

Wenn ein Lead- und ein Kontaktfeld in Salesforce unterschiedliche Werte aufweisen:

1. Wenn Sie einen zusätzlichen Wert in SFDC zu einer Auswahlliste hinzufügen, wird eine Benachrichtigung angezeigt.
1. In der Benachrichtigung erfahren Sie, wo sie verwendet wird. Sie können diesen neuen Wert jetzt bei Bedarf als Option im Formular hinzufügen.

Wenn eine Auswahlliste eines SFDC-Leads andere Werte hat als eine Auswahlliste für einen SFDC-Kontakt, werden die allgemeinen Werte als Standardwertoptionen im Formular verwendet.

Wenn Sie einen Wert aus einer Auswahlliste entfernen, müssen Sie ihn manuell als Option aus Ihren Formularen entfernen.
