---
unique-page-id: 2952636
description: Suchen nach doppelten Personen mit benutzerdefinierter Logik - Marketo-Dokumente - Produktdokumentation
title: Suchen nach doppelten Personen mit benutzerdefinierter Logik
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 13%

---

# Suchen nach doppelten Personen mit benutzerdefinierter Logik {#find-duplicate-people-with-custom-logic}

Marketo Engage verfügt über eine System-Smart-List, mit der doppelte Personen anhand ihrer E-Mail-Adressen gefunden werden. Wenn Sie ein anderes Feld verwenden möchten, um Duplikate mit zu finden, sehen Sie folgendes.

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

   Fertig! Führen Sie die Smart-Liste aus, um Personen mit demselben Wert im zuvor ausgewählten Feld zu finden.
