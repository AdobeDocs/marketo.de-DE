---
description: Verwenden von Massen-Hinzufügen zur Verkaufskampagne in Salesforce - Marketo Docs - Produktdokumentation
title: Verwenden von Massen-Add zu Verkaufskampagnen in Salesforce
exl-id: 49bdd22f-f313-497b-af8d-8308eb905b8f
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Verwenden von Massen-Add zu Verkaufskampagnen in Salesforce {#using-bulk-add-to-sales-campaign-in-salesforce}

Erfahren Sie, wie Sie in Salesforce Bulk zu Sales Campaign hinzufügen können, um Ihre ausgehende Kommunikation mithilfe von Verkaufsaktionen zu skalieren.

>[!NOTE]
>
>Salesforce erzwingt eine Beschränkung von 200 Datensätzen, die gleichzeitig ausgewählt werden können.

>[!PREREQUISITES]
>
>Vergewissern Sie sich, dass Sie die [neuestes Sales Insight-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} in Ihren Kontakt- und Lead-Listenansichten in Salesforce.

## Massen-Hinzufügen zur Verkaufskampagne in Salesforce Lightning {#bulk-add-to-sales-campaign-in-salesforce-lightning}

1. Navigieren Sie in Salesforce zur Startseite Leads/Kontakte , indem Sie auf die Schaltfläche **Leads/Kontakte** Registerkarte.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-1.png)

1. Im **Ansicht** wählen Sie die gewünschte Ansicht der Leads/Kontakte aus, die Sie per E-Mail versenden möchten.

   >[!TIP]
   >
   >Sie können eine neue Ansicht erstellen, indem Sie auf das Zahnradsymbol rechts klicken und **Neu**. Nachdem Sie der Ansicht einen neuen Namen gegeben und gespeichert haben, können Sie auf das Filtersymbol rechts neben der Ansicht klicken, um nach dem gewünschten Satz von Leads/Kontakten zu filtern, die Sie per E-Mail versenden möchten.

1. Wählen Sie die gewünschte Lead- oder Kontaktliste aus und klicken Sie auf die Schaltfläche **Zu Vertriebskampagne hinzufügen** Schaltfläche.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-2.png)

1. Sie werden zum Modal Aktionsverkäufe-Kampagne navigiert, wobei die von Ihnen ausgewählten Empfänger hinzugefügt werden.

1. Nehmen Sie die erforderlichen Änderungen vor, um Personen oder Gruppen zu entfernen. Klicken Sie dann auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-3.png)

1. Wählen Sie aus der Dropdown-Liste Kategorien die Kategorie der Verkaufskampagne aus, die Sie verwenden möchten.

1. Wählen Sie die Verkaufskampagne aus, der Sie die ausgewählten Personen hinzufügen möchten, und klicken Sie auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-4.png)

1. Je nach dem ersten Schritt in Ihrer Kampagne können unterschiedliche Optionen angezeigt werden. Wenn es sich bei Ihrem ersten Schritt um eine E-Mail handelt, können Sie die E-Mail für jeden Empfänger bearbeiten, wie unten dargestellt. Klicken Sie anschließend auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-5.png)

1. Wenn es sich bei Ihrem ersten Schritt um eine E-Mail handelt und Sie diese so konfiguriert haben, dass Sie den Zeitpunkt des Starts der Kampagne auswählen können, haben Sie die Möglichkeit, **Jetzt starten** oder **Planen einer neuen Startzeit**. Klicken Sie nach dem Abschluss auf **Starten**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-6.png)

Nachdem Sie auf Start geklickt haben, wird ein Bestätigungsbildschirm angezeigt, auf dem Sie erfahren, wie viele Personen hinzugefügt wurden.

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-7.png)

## Massen-Hinzufügen zu Vertriebskampagnen in Salesforce Classic {#bulk-add-to-sales-campaign-in-salesforce-classic}

1. Klicken Sie in Salesforce auf die **Leads/Kontakte** Registerkarte.

1. Wählen Sie in der Dropdownliste Ansicht die gewünschte Ansicht der Leads/Kontakte aus, die Sie per E-Mail versenden möchten, und klicken Sie auf **Los**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-8.png)

   >[!TIP]
   >
   >Sie können eine neue Ansicht erstellen, indem Sie auf Neue Ansicht erstellen klicken und die verfügbaren Filter konfigurieren, um die Liste der Empfänger, die Sie per E-Mail versenden, einzugrenzen.

1. Wählen Sie die gewünschte Lead- oder Kontaktliste aus und klicken Sie auf die **Zu Vertriebskampagne hinzufügen** Schaltfläche.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-9.png)

1. Sie werden zum Modal Aktionsverkäufe-Kampagne mit den von Ihnen ausgewählten Personen navigieren.

1. Nehmen Sie die erforderlichen Änderungen vor, um Personen oder Gruppen zu entfernen. Klicken Sie dann auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-10.png)

1. Wählen Sie die Kategorie der Verkaufskampagne aus, die Sie verwenden möchten, indem Sie die **Kategorien** angezeigt.

1. Wählen Sie die Verkaufskampagne aus, der Sie die ausgewählten Personen hinzufügen möchten, und klicken Sie auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-11.png)

1. Je nach dem ersten Schritt in Ihrer Kampagne können unterschiedliche Optionen angezeigt werden. Wenn es sich bei Ihrem ersten Schritt um eine E-Mail handelt, können Sie die E-Mail für jeden Empfänger bearbeiten, wie unten dargestellt. Klicken Sie anschließend auf **Nächste**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-12.png)

1. Wenn es sich bei Ihrem ersten Schritt um eine E-Mail handelt und Sie diese so konfiguriert haben, dass Sie den Zeitpunkt des Starts der Kampagne auswählen können, haben Sie die Möglichkeit, **Jetzt starten** oder **Planen einer neuen Startzeit**. Klicken Sie nach dem Abschluss auf **Starten**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-13.png)

Nachdem Sie auf Start geklickt haben, wird ein Bestätigungsbildschirm angezeigt, auf dem Sie erfahren, wie viele Personen hinzugefügt wurden.

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-14.png)
