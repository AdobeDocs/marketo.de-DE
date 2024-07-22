---
unique-page-id: 2359646
description: Konfigurieren des progressiven Profilings von Formularen - Marketo Docs - Produktdokumentation
title: Konfigurieren des progressiven Profils
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Konfigurieren des progressiven Profils {#configure-form-progressive-profiling}

Kurze Formulare sind gut! Wenn jemand zu einem Formular zurückkehrt, können Sie neue Felder präsentieren und das Profil des Besuchers nach und nach ausfüllen. So geht es.

>[!NOTE]
>
>Damit diese Funktion ordnungsgemäß funktioniert, stellen Sie sicher, dass das Vorfeld &quot;Formular&quot;für sichtbare Felder aktiviert ist und [deaktiviert](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) für ausgeblendete Felder.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Klicken Sie unter &quot;**Formulareinstellungen**&quot;auf &quot;**Einstellungen**&quot;.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Setzen Sie **progressives Profiling** auf **aktiviert**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Okay, nun konfigurieren wir es. Wechseln Sie zu **Felddetails**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Ziehen Sie alle Felder in den Arbeitsbereich, die Teil des progressiven Profilsatzes sind.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Wenn Sie alle Felder verschoben haben, sollte dies etwa so aussehen:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Die Felder außerhalb des Felds **Progressives Profiling** werden immer im Formular angezeigt, auch wenn sie ausgefüllt sind.

1. Wählen Sie das Feld **Progressives Profiling** aus.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Seien Sie bei der Verwendung der erforderlichen Felder in der Progressiven Profilerstellung vorsichtig. Diese Felder können weiterhin leer gelassen werden, wenn der Besucher eine neue E-Mail-Adresse eingibt (wodurch eine neue Person erstellt würde), nachdem er zuvor Daten für die anderen Felder gesendet hat, da sie auf dem neuesten Formular unterdrückt würden.

1. Wählen Sie nun aus dem Feld **Progressives Profiling** aus, wie viele leere Felder angezeigt werden sollen.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Wenn Sie **Zahl** **von** **Leer** **Felder** als 1 auswählen, wird dem Besucher beim ersten Mal dieses Formular angezeigt:
   >
   >* Vorname (leer)
   >* Nachname (leer)
   >* E-Mail-Adresse (leer)
   >* Telefonnummer (leer)
   >
   >Wenn sie jedes Feld ausfüllen, sehen sie beim zweiten Besuch Folgendes:
   >
   >* Vorname (vorausgefüllt)
   >* Nachname (vorausgefüllt)
   >* E-Mail-Adresse (vorausgefüllt)
   >* Mobiltelefonnummer (leer)
   >
   >Wenn sie die Mobiltelefonnummer ausfüllen, sehen sie beim dritten Besuch Folgendes:
   >
   >* Vorname (vorausgefüllt)
   >* Nachname (vorausgefüllt)
   >* E-Mail-Adresse (vorausgefüllt)
   >* Land (leer)

1. Klicken Sie auf **Beenden**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Klicken Sie auf **Genehmigen und schließen**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Gut gemacht! Die Arbeit, die du gerade gemacht hast, wird sich lohnen.

Experimentieren Sie mit dieser Funktion und testen Sie unbedingt. Es ist erweitert, aber Sie können Ihre Formulare auf diese Weise sehr dynamisch machen.
