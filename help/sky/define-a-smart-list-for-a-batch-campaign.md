---
title: define-a-smart-Liste-for-a-batch-Kampagne
description: Definieren einer intelligenten Liste für eine Batch-Kampagne
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Definieren einer intelligenten Liste für eine Batch-Kampagne

<br> 

Intelligente Listen sind der Mechanismus in Marketo, um zu definieren, wer (welche Personen) eingeschlossen werden soll, ob es sich um einen Bericht, eine Liste oder eine intelligente Kampagne handelt. So definieren Sie eine intelligente Liste für eine Batch-Kampagne.

1. Wählen Sie eine intelligente Kampagne und klicken Sie dann auf **[!UICONTROL Intelligente Liste]**.

   ![Bild eins](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Geben Sie ein, um nach einem Filter zu suchen, und ziehen Sie ihn per Drag &amp; Drop auf die Arbeitsfläche. Wiederholen Sie diese Schritte für mehrere Filter.

   ![Bild zwei](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Eine intelligente Kampagne mit nur Filtern wird im Stapelmodus ausgeführt. Es findet Personen in der Datenbank, die sich auf Grundlage der Filter qualifizieren, und führt sie alle gleichzeitig durch den Fluss.

   >[!IMPORTANT]
   >
   >Sie können eine intelligente Kampagne auf der Grundlage von Live-Ereignissen einzeln ausführen lassen, indem Sie Trigger hinzufügen, wodurch die intelligente Kampagne im Trigger-Modus ausgeführt wird.

1. Klicken Sie auf die Dropdownliste und wählen Sie einen Filteroperator (z. B. **[!UICONTROL ist]**, **[!UICONTROL ist nicht]** usw.) für den ausgewählten Filter.

   ![Bild drei](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Rote Linien weisen auf Fehler oder fehlende Informationen hin. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

1. Geben Sie den Filterwert ein.

   ![Bild vier](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Standardmäßig sind Personen, die ALLE Regeln der intelligenten Liste erfüllen,
>qualifiziert. Dies kann an Ihre Kampagne angepasst werden. Weitere Informationen finden Sie unter [Intelligente Liste für Complex Logic](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic).
>
>Um auf Live-Ereignissen einzeln Trigger, lernen Sie [Intelligente Liste für intelligente Kampagne definieren. | Trigger](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
