---
unique-page-id: 2359646
description: Konfigurieren der progressiven Profilerstellung - Marketing Docs - Produktdokumentation
title: Konfigurieren der progressiven Profilerstellung
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Konfigurieren der progressiven Profilerstellung {#configure-form-progressive-profiling}

Kurze Formulare sind gut! Wenn jemand zu einem Formular zurückkehrt, können Sie neue Felder präsentieren und das Profil des Besuchers schrittweise ausfüllen. So geht es.

>[!NOTE]
>
>Damit diese Funktion ordnungsgemäß funktioniert, müssen Sie sicherstellen, dass das Vorausfüllen des Formulars für sichtbare Felder aktiviert und für ausgeblendete Felder [deaktiviert](http://docs.marketo.com/display/DOCS/Disable+Pre-fill+for+a+Form+Field) ist.

1. Gehen Sie zu **Marketing** - **Aktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Bearbeiten** des **Formulars**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Klicken Sie unter **Formulareinstellungen** auf **Einstellungen****Einstellungen**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Legen Sie **Progressive** **Profiling** auf **Aktiviert** fest.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Okay, jetzt konfigurieren wir es. Zu **Felddetails** **gehen**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)
Ziehen Sie per Drag &amp; Drop alle Felder, die Teil des progressiven Profils sind.
   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Wenn Sie alle Felder verschoben haben, sollte es wie folgt aussehen:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Die Felder außerhalb des **Feldes Progressive** **Profiling** werden immer im Formular angezeigt, auch wenn sie ausgefüllt sind.

1. Wählen Sie das Feld **Progressives** **Profiling** .

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Seien Sie vorsichtig, wenn Sie die erforderlichen Felder in der Progressiven Profilerstellung verwenden. Diese Felder können weiterhin leer gelassen werden, wenn der Besucher eine neue E-Mail-Adresse eingibt (wodurch eine neue Person erstellt würde), nachdem zuvor Daten für die anderen Felder übermittelt wurden, da sie im neuesten Formular unterdrückt würden.

1. Wählen Sie jetzt aus dem Feld **Progressives** **Profiling** aus, wie viele leere Felder angezeigt werden sollen.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >
   >Wenn Sie **Anzahl** **der** leeren **** Felder **** als 1 auswählen, wird dem Besucher beim ersten Anzeigen dieses Formulars Folgendes angezeigt:
   >
   >    
   >    
   >    * Vorname (leer)
   >    * Nachname (leer)
   >    * E-Mail-Adresse (leer)
   >    * Telefonnummer (leer)

   >    
   >    
   >Wenn sie jedes Feld ausfüllen, sehen sie beim zweiten Besuch Folgendes:
   >
   >    
   >    
   >    * Vorname (vorausgefüllt)
   >    * Nachname (vorausgefüllt)
   >    * E-Mail-Adresse (vorausgefüllt)
   >    * Mobiltelefonnummer (leer)

   >    
   >    
   >Wenn sie die Nummer des Mobiltelefons ausfüllen, sehen sie beim dritten Besuch Folgendes:
   >
   >    
   >    
   >    * Vorname (vorausgefüllt)
   >    * Nachname (vorausgefüllt)
   >    * E-Mail-Adresse (vorausgefüllt)
   >    * Land (leer)


1. Klicken Sie auf **Fertig stellen**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Klicken Sie auf **Genehmigen und Schließen**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Gute Arbeit! Die Arbeit, die du gerade gemacht hast, wird sich lohnen.

Experimentieren Sie mit dieser Funktion und testen Sie sie. Es ist fortschrittlich, aber Sie können Ihre Formulare auf diese Weise sehr dynamisch gestalten.
