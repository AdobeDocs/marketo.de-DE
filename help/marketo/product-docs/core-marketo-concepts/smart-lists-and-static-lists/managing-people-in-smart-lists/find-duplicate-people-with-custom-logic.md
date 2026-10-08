---
unique-page-id: 2952636
description: Erfahren Sie, wie Sie doppelte Personen mit benutzerdefinierter Logik finden. Erstellen Sie eine Smart List, um Duplikate anhand Ihrer Kriterien zu identifizieren.
title: Suchen nach doppelten Personen mit benutzerdefinierter Logik
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 12%
---
# Suchen nach doppelten Personen mit benutzerdefinierter Logik {#find-duplicate-people-with-custom-logic}

Marketo Engage verfügt über eine System-Smart-List, mit der doppelte Personen anhand ihrer E-Mail-Adressen gefunden werden. Wenn Sie Duplikate mit einem anderen Feld suchen möchten, führen Sie die folgenden Schritte aus.

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Navigieren Sie zum Bereich **[!UICONTROL Marketing-Aktivitäten]**.

![](assets/ma-2.png)

1. Wählen Sie Ihre Smart-Liste aus und klicken Sie auf die Registerkarte **[!UICONTROL Smart-Liste]**.

   ![](assets/two-4.png)

1. Suchen Sie den Filter **[!UICONTROL Felder duplizieren]** und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/three-4.png)

1. Wählen Sie eine von vier verfügbaren Optionen:

   * [!UICONTROL E-Mail-]
   * [!UICONTROL Vollständiger Name]
   * [!UICONTROL Nachname]
   * [!UICONTROL Aktualisiert um]

   >[!NOTE]
   >
   >Bei allen Feldern mit Ausnahme der E-Mail-Adresse wird zwischen Groß- und Kleinschreibung unterschieden. Wenn Sie also „Martin Müller“ im Feld Vollständiger Name verwenden _werden_ Ergebnisse für Martin Müller zurückgegeben.

   ![](assets/four-2.png)

   Führen Sie die Smart-Liste aus, um Personen mit demselben Wert im zuvor ausgewählten Feld zu finden.
