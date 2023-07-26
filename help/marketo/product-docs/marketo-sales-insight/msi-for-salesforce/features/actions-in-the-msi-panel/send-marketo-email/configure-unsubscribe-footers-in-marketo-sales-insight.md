---
unique-page-id: 2953373
description: Konfigurieren von Abmeldefußzeilen in Marketo Sales Insight - Marketo Docs - Produktdokumentation
title: Konfigurieren von Abmeldefußzeilen in Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 2%

---

# Konfigurieren von Abmeldefußzeilen in Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

In E-Mails zum Verkauf wird die Abmelde-Fußzeile automatisch am unteren Rand platziert. Sie können die Einstellungen jedoch an Ihre Anforderungen anpassen.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>**Definition**
>
>**Verkaufs-E-Mails** sind diejenigen, die von Sales Insight gesendet werden (nicht enthalten sind diejenigen, die vom Marketo Outlook-Plugin gesendet werden).

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/one-1.png)

1. Klicks **Sales Insight**, dann **Einstellungen bearbeiten**.

   ![](assets/two-1.png)

   Es gibt mehrere Möglichkeiten. Sehen wir uns zunächst die E-Mail-Typen an, für die Sie die Einstellungen ändern können.

   ![](assets/three-1.png)

   * **Keine Vorlage** - Manuell von einem Vertriebsbenutzer erstellt.
   * **Standard-Email** - Vorlagen für E-Mails.
   * **Operative E-Mail** - E-Mails, die Abmeldungen ignorieren, Marketing ausgesetzt und Kommunikationsbeschränkungen (unabhängig davon, was gesendet wird).

   Sie können für jeden Typ ein anderes Verhalten festlegen.

   >[!CAUTION]
   >
   >**Abmeldeeinstellungen respektieren**: abgemeldete Leads erhalten die E-Mail NICHT, selbst wenn die veröffentlichte E-Mail &quot;funktionsfähig&quot;ist.
   >
   >**Ignorieren von Abmeldeeinstellungen**: abgemeldete Leads erhalten die E-Mail

1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie dann auf **Speichern**.

   >[!TIP]
   >
   >Die letzten beiden Optionen ermöglichen es, die Abmeldefußzeile dynamisch einzuschließen/auszuschließen, je nach Empfängeranzahl (größer als 1 oder größer als 5).

   ![](assets/four-1.png)

Egal! Ein wenig kompliziert, aber ziemlich flexibel, nicht wahr?
