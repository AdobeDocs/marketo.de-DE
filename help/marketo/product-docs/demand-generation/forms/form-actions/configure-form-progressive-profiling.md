---
unique-page-id: 2359646
description: Konfigurieren der progressiven Formularprofilerstellung - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren der progressiven Formularprofilerstellung
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Konfigurieren der progressiven Formularprofilerstellung {#configure-form-progressive-profiling}

Kurze Formulare sind gut! Wenn jemand zu einem Formular zurückkehrt, können Sie neue Felder präsentieren und schrittweise das Profil des Besuchers ausfüllen. So geht&#39;s.

>[!NOTE]
>
>Damit diese Funktion ordnungsgemäß funktioniert, müssen Sie sicherstellen, dass das Vorausfüllen des Formulars für sichtbare Felder und [deaktiviert](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) für ausgeblendete Felder aktiviert ist.

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma-1.png)

1. Wählen Sie Ihr Formular aus und klicken Sie auf **[!UICONTROL Formular bearbeiten]**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Legen Sie **[!UICONTROL Progressive Profiling]** auf **[!UICONTROL Aktiviert]** fest.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Okay, konfigurieren wir es jetzt. Wechseln Sie zu **[!UICONTROL Felddetails]**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Ziehen Sie alle Felder, die Teil des progressiven Profilsatzes sind, per Drag-and-Drop.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Wenn Sie alle Felder verschieben, sollte es in etwa so aussehen:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Die Felder außerhalb des Felds **[!UICONTROL Progressive Profiling]** werden immer im Formular angezeigt, auch wenn sie ausgefüllt sind.

1. Aktivieren Sie das **[!UICONTROL Progressive Profiling]**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Seien Sie vorsichtig, wenn Sie erforderliche Felder in [!UICONTROL Progressive Profiling] verwenden. Diese Felder können weiterhin leer gelassen werden, wenn der Besucher eine neue E-Mail-Adresse eingibt (wodurch eine neue Person erstellt wird), nachdem er zuvor Daten für die anderen Felder übermittelt hat, da diese auf dem neuesten Formular unterdrückt würden.

1. Wählen Sie jetzt aus dem Feld „Progressive Profiling **aus, wie viele leere Felder** Personen gleichzeitig angezeigt werden sollen.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Wenn Sie **[!UICONTROL Anzahl leerer Felder]** als 1 auswählen, wird dem Besucher bei der ersten Anzeige dieses Formulars Folgendes angezeigt:
   >
   >* Vorname (leer)
   >* Nachname (leer)
   >* E-Mail-Adresse (leer)
   >* Telefonnummer (leer)
   >
   >Wenn sie jedes Feld ausfüllen, werden sie beim zweiten Besuch Folgendes sehen:
   >
   >* Vorname (vorbefüllt)
   >* Nachname (vorbefüllt)
   >* E-Mail-Adresse (vorbefüllt)
   >* Mobiltelefonnummer (leer)
   >
   >Wenn sie die Mobiltelefonnummer angeben, sehen sie beim dritten Besuch Folgendes:
   >
   >* Vorname (vorbefüllt)
   >* Nachname (vorbefüllt)
   >* E-Mail-Adresse (vorbefüllt)
   >* Land (leer)

1. Klicken Sie auf **[!UICONTROL Fertigstellen]**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Klicken Sie **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Gute Arbeit! Die Arbeit, die Sie gerade getan haben, wird sich auszahlen.

Experimentieren Sie mit dieser Funktion und stellen Sie sicher, dass Sie sie testen. Es ist sehr fortgeschritten, aber Sie können auf diese Weise Ihre Formulare sehr dynamisch machen.
