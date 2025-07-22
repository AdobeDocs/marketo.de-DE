---
unique-page-id: 12983101
description: Zuordnen benutzerdefinierter Felder zu Marketo - Marketo-Dokumente - Produktdokumentation
title: Zuordnen benutzerdefinierter Felder zu Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Zuordnen benutzerdefinierter Felder zu Marketo {#map-custom-fields-to-marketo}

Sie möchten möglicherweise mehr als die standardmäßigen Informationen erfassen, die standardmäßig gespeichert [!DNL Facebook], z. B. wie oft jemand Ihren Online-Versanddienst verwendet. Sie können dies erreichen, indem [benutzerdefinierte Fragen erstellen](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) in Ihren [!DNL Facebook]-Lead-Anzeigen verwenden.

**Marketo beginnt jedoch nicht automatisch mit der Erfassung dieser Daten**. Damit Marketo mit der Erfassung benutzerdefinierter Feldwerte beginnen kann, **müssen** diese benutzerdefinierten Felder einem Feld in Marketo zugeordnet werden.

Gehen Sie wie folgt vor, um dies im LaunchPoint-Bereich von Admin einzurichten.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Wechseln Sie zum Bereich Admin und klicken Sie auf **[!UICONTROL LaunchPoint]**. Suchen und bearbeiten Sie unter Installierte Dienste **[!UICONTROL Facebook-Lead-Anzeigen]**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Lassen Sie das autorisierte Konto unverändert - nehmen Sie **Änderungen** vor. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Belassen Sie die ausgewählten Seiten unverändert und nehmen Sie **Änderungen**. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Hier ordnen Sie das benutzerdefinierte [!DNL Facebook] Ihrem Marketo-Feld zu. Klicken Sie auf **[!UICONTROL Hinzufügen].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Geben Sie in der neuen Zeile den Namen Ihres [!DNL Facebook] benutzerdefinierten Felds ein.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Nur Felder, die in [!DNL Facebook] Formularvorlagen gespeichert wurden, werden hier als Optionen angezeigt.

1. Klicken Sie in die Spalte **[!UICONTROL Marketo]**. Tippen Sie, um nach dem Feld zu suchen, dem Sie zuordnen möchten. Klicken Sie nach Auswahl eines Felds auf **[!UICONTROL Speichern]**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Wenn Sie noch kein Feld in Marketo haben, dem Sie das [!DNL Facebook] zuordnen können, erfahren Sie, wie Sie [benutzerdefinierte Felder erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Sie **müssen** diesen Prozess für jedes neue [!DNL Facebook] durchführen, damit Marketo die Daten erfassen kann.
