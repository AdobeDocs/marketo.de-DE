---
unique-page-id: 2953373
description: Konfigurieren von Abmelde-Fußzeilen in Marketo Sales Insight - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren von Abmelde-Fußzeilen in Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Konfigurieren von Abmelde-Fußzeilen in Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Bei Verkaufs-E-Mails wird die Fußzeile zur Abmeldung automatisch unten angezeigt. Sie können die Einstellungen jedoch an Ihre Anforderungen anpassen.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>**Definition**
>
>**Verkaufs-E** Mails sind die, die von Sales Insight gesendet werden (sie umfassen nicht die vom Marketo Outlook-Plug-in gesendeten).

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/one-1.png)

1. Klicken Sie **Sales Insight** und dann **Einstellungen bearbeiten**.

   ![](assets/two-1.png)

   Es gibt mehrere Möglichkeiten. Im Folgenden werden zunächst die E-Mail-Typen beschrieben, für die Sie die Einstellungen ändern können.

   ![](assets/three-1.png)

   * **Keine Vorlage** - Manuell vom Verkaufsbenutzer erstellt.
   * **Standard-E-**: E-Mails, die auf einer Vorlage basieren.
   * **Operative E-**: E-Mails, die die Beschränkungen für Abgemeldetes, ausgesetztes Marketing und Kommunikation ignorieren (sie senden unabhängig davon, was passiert).

   Sie haben die Möglichkeit, für jeden Typ ein anderes Verhalten festzulegen.

   >[!CAUTION]
   >
   >**Abmeldeeinstellungen respektieren**: Abgemeldete Leads erhalten die E-Mail NICHT, selbst wenn die veröffentlichte E-Mail „betriebsbereit“ ist
   >
   >**Abmeldeeinstellungen ignorieren**: Abgemeldete Leads erhalten die E-Mail

1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie dann auf **Speichern**.

   >[!TIP]
   >
   >Mit den letzten beiden Optionen können Sie die Abmelde-Fußzeile je nach Anzahl der Empfänger (größer als 1 oder größer als 5) dynamisch ein- oder ausschließen.

   ![](assets/four-1.png)

Wau! Ein bisschen kompliziert, aber ziemlich flexibel, oder?
