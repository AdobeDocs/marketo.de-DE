---
unique-page-id: 2952636
description: Suchen doppelter Personen mit benutzerdefinierter Logik - Marketo-Dokumente - Produktdokumentation
title: Duplizierte Personen mit benutzerdefinierter Logik suchen
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 5%

---

# Duplizierte Personen mit benutzerdefinierter Logik suchen {#find-duplicate-people-with-custom-logic}

Marketo Engage verfügt über eine System-Smart-Liste, die anhand der E-Mail-Adressen doppelte Personen findet. Wenn Sie ein anderes Feld verwenden möchten, um Duplikate mit zu finden, können Sie dies folgendermaßen tun:

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Wechseln Sie zum Bereich **[!UICONTROL Marketingaktivitäten]** .

![](assets/ma-2.png)

1. Wählen Sie Ihre Smart-Liste aus und klicken Sie auf die Registerkarte **[!UICONTROL Smart-Liste]** .

   ![](assets/two-4.png)

1. Suchen und ziehen Sie den Filter **[!UICONTROL Duplizierte Felder]** auf die Arbeitsfläche.

   ![](assets/three-4.png)

1. Wählen Sie eine von vier verfügbaren Optionen aus:

   * E-Mail-Adresse
   * Vollständiger Name
   * Nachname
   * Aktualisiert um

   >[!NOTE]
   >
   >Bei allen Feldern außer E-Mail-Adresse wird zwischen Groß- und Kleinschreibung unterschieden. Wenn Sie also &quot;john doe&quot;im Feld &quot;Full Name&quot;verwenden, werden für John Doe _nicht_ Ergebnisse zurückgegeben.

   ![](assets/four-2.png)

   Fertig! Führen Sie die Smart-Liste aus, um Personen mit demselben Wert im zuvor ausgewählten Feld zu suchen.
