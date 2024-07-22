---
unique-page-id: 2951220
description: Erstellen eines Personenleistungsberichts mit Mobile Platform-Spalten - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Personenleistungsberichts mit Mobile Platform-Spalten
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Erstellen eines Personenleistungsberichts mit Mobile Platform-Spalten {#build-a-people-performance-report-with-mobile-platform-columns}

Führen Sie diese Schritte aus, um einen Bericht zur Leistung für Personen mit mobilen Plattformen (iOS/Android) zu erstellen.

## Erstellen mobiler Smart-Listen {#create-mobile-smart-lists}

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie ein Programm.

   ![](assets/two-1.png)

1. Wählen Sie unter &quot;**Neu**&quot;die Option &quot;**Neues lokales Asset**&quot;.

   ![](assets/three-1.png)

1. Klicken Sie auf **Smart List**.

   ![](assets/four-1.png)

1. Geben Sie einen Namen ein und klicken Sie auf **Erstellen**.

   ![](assets/five-1.png)

1. Suchen und ziehen Sie den Filter Geöffnete E-Mail in die Arbeitsfläche.

   ![](assets/six-1.png)

1. Setzen Sie E-Mail auf &quot;**ist beliebig**&quot;.

   ![](assets/seven.png)

1. Klicken Sie auf **Beschränkung hinzufügen** und wählen Sie **Plattform** aus.

   ![](assets/eight.png)

   >[!TIP]
   >
   >In diesem Beispiel haben wir den Filter Geöffnete E-Mail verwendet. Sie können auch den Filter &quot;Angeklickte E-Mail&quot;verwenden, da er die Platform-Beschränkung aufweist.

1. Setzen Sie Platform auf **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Mindestens eine Person muss eine Ihrer E-Mails auf einem iOS-Gerät geöffnet haben, damit Marketo sie automatisch finden kann. Wenn sie nicht angezeigt wird, können Sie sie manuell eingeben und speichern.

   Erstellen Sie nun eine zweite Smart-Liste für die Plattform &quot;Android&quot;. Fahren Sie nach Abschluss des Vorgangs mit dem nächsten Abschnitt fort.

## Erstellen eines Berichts zur Leistung von Personen {#create-a-people-performance-report}

1. Wählen Sie unter Marketingaktivitäten das Programm aus, in dem Ihre Smart-Listen **iOS** und **Android** enthalten sind.

   ![](assets/ten.png)

1. Wählen Sie unter &quot;**Neu**&quot;die Option &quot;**Neues lokales Asset**&quot;.

   ![](assets/eleven.png)

1. Klicken Sie auf **Bericht**.

   ![](assets/twelve.png)

1. Setzen Sie den Typ auf **Leistung von Personen**.

   ![](assets/thirteen.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/fourteen.png)

   Es geht dir gut! Nun zum nächsten Abschnitt.

## Mobile Smart-Listen als Spalten hinzufügen {#add-mobile-smart-lists-as-columns}

1. Klicken Sie im soeben erstellten Bericht auf **Einrichtung** und ziehen Sie dann **Benutzerdefinierte Spalten** auf die Arbeitsfläche.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Der Bericht &quot;Personen-Performance&quot;bezieht sich standardmäßig auf die letzten 7 Tage. Sie können den Zeitraum ändern, indem Sie darauf doppelklicken.

1. Suchen und wählen Sie die zuvor erstellten Smart-Listen aus und klicken Sie auf **Anwenden**.

   ![](assets/sixteen.png)

1. Klicken Sie auf **Bericht** , um den Bericht auszuführen und Ihre Daten anzuzeigen.

   ![](assets/seventeen.png)

   Ziemlich cool, nicht wahr? Schön gemacht!
