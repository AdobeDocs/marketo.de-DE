---
unique-page-id: 2952636
description: Suchen doppelter Personen mit benutzerdefinierter Logik - Marketo-Dokumente - Produktdokumentation
title: Duplizierte Personen mit benutzerdefinierter Logik suchen
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# Duplizierte Personen mit benutzerdefinierter Logik suchen {#find-duplicate-people-with-custom-logic}

Marketo verfügt über eine System-Smart-Liste, die anhand der E-Mail-Adressen doppelte Personen findet. Wenn Sie ein anderes Feld verwenden möchten, um Duplikate mit zu finden, können Sie dies folgendermaßen tun:

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Navigieren Sie zu **Marketingaktivitäten** Bereich.

![](assets/ma-2.png)

1. Wählen Sie Ihre Smart-Liste aus und klicken Sie auf die **Smart List** Registerkarte.

   ![](assets/two-4.png)

1. Suchen und Ziehen **Felder duplizieren** auf die Arbeitsfläche.

   ![](assets/three-4.png)

1. Wählen Sie eine von vier verfügbaren Optionen aus:

   * E-Mail-Adresse
   * Vollständiger Name
   * Nachname
   * Aktualisiert am

   >[!NOTE]
   >
   >Bei allen Feldern außer E-Mail-Adresse wird zwischen Groß- und Kleinschreibung unterschieden. Die Verwendung von &quot;john doe&quot;im Feld &quot;Vollständiger Name&quot;würde _not_ Ergebnisse für John Doe zurückgeben.

   ![](assets/four-2.png)

   Abgeschlossen! Führen Sie die Smart-Liste aus, um Personen mit demselben Wert im zuvor ausgewählten Feld zu finden.
