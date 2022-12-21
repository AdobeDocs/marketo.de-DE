---
unique-page-id: 2359646
description: Konfigurieren des progressiven Profilings von Formularen - Marketo Docs - Produktdokumentation
title: Konfigurieren des progressiven Profils
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Konfigurieren des progressiven Profils {#configure-form-progressive-profiling}

Kurze Formulare sind gut! Wenn jemand zu einem Formular zurückkehrt, können Sie neue Felder präsentieren und das Profil des Besuchers nach und nach ausfüllen. So geht es.

>[!NOTE]
>
>Damit diese Funktion ordnungsgemäß funktioniert, stellen Sie sicher, dass das Vorfeld &quot;Formular ausfüllen&quot;für sichtbare Felder aktiviert ist, und [disabled](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) für ausgeblendete Felder.

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. under **Formulareinstellungen** klicken **Einstellungen**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Satz **Progressives Profiling** nach **Aktiviert**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Okay, nun konfigurieren wir es. Navigieren Sie zu **Felddetails**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Ziehen Sie alle Felder in den Arbeitsbereich, die Teil des progressiven Profilsatzes sind.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Wenn Sie alle Felder verschoben haben, sollte dies etwa so aussehen:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Die Felder außerhalb der **Progressives Profiling** wird immer im Formular angezeigt, auch wenn sie ausgefüllt sind.

1. Wählen Sie die **Progressives Profiling** ankreuzen.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Seien Sie bei der Verwendung der erforderlichen Felder in der Progressiven Profilerstellung vorsichtig. Diese Felder können weiterhin leer gelassen werden, wenn der Besucher eine neue E-Mail-Adresse eingibt (wodurch eine neue Person erstellt würde), nachdem er zuvor Daten für die anderen Felder gesendet hat, da sie auf dem neuesten Formular unterdrückt würden.

1. Wählen Sie nun aus dem **Progressives Profiling** jedes Mal.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Wenn Sie **Zahl** **von** **Leer** **Felder** den Wert 1 hat, sieht der Besucher Folgendes, wenn er dieses Formular zum ersten Mal sieht:
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


1. Klicken **Beenden**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Klicken **Genehmigen und schließen**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Gut gemacht! Die Arbeit, die du gerade gemacht hast, wird sich lohnen.

Experimentieren Sie mit dieser Funktion und testen Sie unbedingt. Es ist erweitert, aber Sie können Ihre Formulare auf diese Weise sehr dynamisch machen.
