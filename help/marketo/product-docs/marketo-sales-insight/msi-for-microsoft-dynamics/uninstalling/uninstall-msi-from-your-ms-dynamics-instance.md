---
unique-page-id: 37355600
description: MSI von Ihrer MS Dynamics-Instanz deinstallieren - Marketo-Dokumente - Produktdokumentation
title: MSI von der MS Dynamics-Instanz deinstallieren
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# MSI von der MS Dynamics-Instanz deinstallieren {#uninstall-msi-from-your-ms-dynamics-instance}

Um MSI aus Ihrer MS Dynamics-Instanz zu deinstallieren, müssen Sie Schritte sowohl in Marketo als auch in MS Dynamics ausführen.

>[!PREREQUISITES]
>
>[Globale MS Dynamics-Synchronisierung deaktivieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one-1.png)

1. Klicken Sie **Sales Insight**.

   ![](assets/six.png)

1. Klicken Sie **Feldsynchronisierung bearbeiten**.

   ![](assets/seven.png)

1. Aktivieren Sie das Kontrollkästchen **Synchronisierung deaktivieren** und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Stellen Sie sicher[ dass Sie die globale MS Dynamics-](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) deaktivieren, bevor Sie die Feldsynchronisierung deaktivieren.

   ![](assets/eight.png)

## Folgende Schritte finden in Ihrer MS Dynamics-Instanz statt: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Klicken Sie **Erweiterte Einstellungen**.

1. Klicken Sie auf **Lösungen**.

1. Wählen Sie **Marketo Sales Insight** aus und klicken Sie auf das Löschsymbol.

1. Wenn das Modal „Lösung deinstallieren“ angezeigt wird, klicken Sie auf **OK**.

   Normalerweise dauert es etwa 20 Minuten, bis die MS Dynamics-Lösung vollständig deinstalliert ist. Wenn Sie jedoch über eine große MS Dynamics-Instanz verfügen, kann dies etwas länger dauern.

   >[!NOTE]
   >
   >Denken Sie daran, die globale MS Dynamics-Synchronisation einzuschalten, sobald Sie MSI deinstallieren.
