---
unique-page-id: 37355600
description: Deinstallieren von MSI von Ihrer MS Dynamics-Instanz - Marketo Docs - Produktdokumentation
title: Deinstallieren von MSI aus Ihrer MS Dynamics-Instanz
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Deinstallieren von MSI aus Ihrer MS Dynamics-Instanz {#uninstall-msi-from-your-ms-dynamics-instance}

Um MSI aus Ihrer MS Dynamics-Instanz zu deinstallieren, müssen Sie Schritte sowohl in Marketo als auch in MS Dynamics durchführen.

>[!PREREQUISITES]
>
>[Globale MS Dynamics-Synchronisierung deaktivieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one-1.png)

1. Klicken **Sales Insight**.

   ![](assets/six.png)

1. Klicken **Feldsynchronisierung bearbeiten**.

   ![](assets/seven.png)

1. Wählen Sie die **Synchronisierung deaktivieren** Kontrollkästchen und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass [Deaktivieren der globalen MS Dynamics-Synchronisierung](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) vor der Deaktivierung der Feldsynchronisierung.

   ![](assets/eight.png)

## Die folgenden Schritte finden in Ihrer MS Dynamics-Instanz statt: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Klicken **Erweiterte Einstellungen**.

1. Klicken **Lösungen**.

1. Auswählen **Marketo Sales Insight** und klicken Sie auf das Löschsymbol.

1. Wenn das Modal Lösung deinstallieren angezeigt wird, klicken Sie auf **OK**.

   Die vollständige Deinstallation der MS Dynamics-Lösung dauert in der Regel etwa 20 Minuten. Wenn Sie jedoch eine große MS Dynamics-Instanz haben, kann es etwas länger dauern.

   >[!NOTE]
   >
   >Denken Sie daran, die Synchronisation von Global MS Dynamics nach der Deinstallation von MSI zu aktivieren.
