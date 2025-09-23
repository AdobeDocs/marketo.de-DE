---
unique-page-id: 2953384
description: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 3%

---

# Aktivieren der Synchronisierung für eine benutzerdefinierte Entität {#enable-sync-for-a-custom-entity}

Wenn benutzerdefinierte Entitätsdaten aus [!DNL Dynamics] in Marketo Engage verfügbar sein sollen, sehen Sie hier, wie Sie die Synchronisierung dafür aktivieren.

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [Lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}-, [Kontakt](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"}- oder [Konto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"}-Objekt in Microsoft Dynamics verknüpft sein.

>[!NOTE]
>
>* Wenn Sie die Synchronisierung für eine benutzerdefinierte Entität aktivieren, führt Marketo eine Erstsynchronisierung durch, um alle Daten für das benutzerdefinierte Objekt einzubringen.
>* Mitglieder von Marketing-Listen und Marketing-Listen _derzeit nicht_.

>[!IMPORTANT]
>
>Der Marketo-Synchronisierungsbenutzer benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung mit ihm durchzuführen.

1. Navigieren Sie zum Abschnitt **[!UICONTROL Admin]**.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Wählen Sie **[!UICONTROL Microsoft Dynamics]** aus und klicken Sie auf **[!UICONTROL Synchronisierung deaktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um eine benutzerdefinierte Entität zu aktivieren oder zu deaktivieren.

1. Klicken [!UICONTROL  unter &quot;]&quot; auf den Link **[!UICONTROL Synchronisierung von Dynamics]** Entitäten.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicken Sie auf den **[!UICONTROL Synchronisierungsschema]**-Link.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Wählen Sie die zu synchronisierende Entität aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Wählen Sie die Felder aus, die Sie synchronisieren oder als [Einschränkungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) und/oder Trigger in Smart-Listen verwenden möchten. Klicken Sie abschließend auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Während des Synchronisierungsvorgangs werden Sie möglicherweise feststellen, dass das Element [!UICONTROL Dynamische Entitäten synchronisieren] aus der Navigationsstruktur verschwindet. Dieses Verhalten ist zu erwarten und wird nach Abschluss der Synchronisierung erneut angezeigt.

1. Die Entität weist jetzt ein grünes Häkchen auf.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardelementen eine oder zwei Ebenen tief verknüpft sind.
   >
   >* Der benutzerdefinierte Objektbaum kann dasselbe Objekt mehrmals anzeigen, da es direkt mit einem der Hauptobjekte verbunden ist (z. B. Leads, Kontakte, Konten oder indirekte Verbindungen über ein Zwischenobjekt). Wählen Sie in solchen Fällen das Objekt aus, das dem Hauptobjekt am nächsten ist, und wählen Sie nur eines. Die mehrfache Auswahl desselben Objekts kann die Synchronisierung dieses benutzerdefinierten Objekts beeinträchtigen.
