---
unique-page-id: 2951220
description: Erstellen eines Leistungsberichts für Personen mit Spalten der mobilen Plattform - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Personenleistungsberichts mit Spalten einer mobilen Plattform
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 6%

---

# Erstellen eines Personenleistungsberichts mit Spalten einer mobilen Plattform {#build-a-people-performance-report-with-mobile-platform-columns}

Führen Sie die folgenden Schritte aus, um einen Leistungsbericht für Personen mit den Spalten für Mobile Platform (iOS/Android) zu erstellen.

## Erstellen von Smart-Listen für Mobilgeräte {#create-mobile-smart-lists}

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma.png)

1. Wählen Sie ein Programm.

   ![](assets/two-1.png)

1. Wählen **[!UICONTROL unter]** die Option **[!UICONTROL Neues lokales Asset]** aus.

   ![](assets/three-1.png)

1. Klicken Sie **[!UICONTROL Smart-Liste]**.

   ![](assets/four-1.png)

1. Geben Sie einen Namen ein und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/five-1.png)

1. Suchen Sie den Filter [!UICONTROL Geöffnete E-Mail] und ziehen Sie ihn in die Arbeitsfläche.

   ![](assets/six-1.png)

1. E-Mail auf **[!UICONTROL ist beliebig]** setzen

   ![](assets/seven.png)

1. Klicken Sie auf **[!UICONTROL Begrenzung hinzufügen]** und wählen Sie **[!UICONTROL Platform]** aus.

   ![](assets/eight.png)

   >[!TIP]
   >
   >In diesem Beispiel haben wir den Filter [!UICONTROL Geöffnete E]Mail“ verwendet. Sie können auch den Filter [!UICONTROL Klickte E-Mail] verwenden, da er die Plattformeinschränkung aufweist.

1. Legen Sie [!UICONTROL Platform] auf **[!UICONTROL iOS]** fest.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Mindestens eine Person muss eine Ihrer E-Mails auf einem iOS-Gerät geöffnet haben, damit Marketos AutoSuggest sie findet. Wenn er nicht angezeigt wird, können Sie ihn manuell eingeben und speichern.

   Erstellen Sie nun eine zweite Smart-Liste für die Plattform &quot;Android&quot;. Fahren Sie nach Abschluss des Vorgangs mit dem nächsten Abschnitt fort.

## Erstellen eines Personenleistungsberichts {#create-a-people-performance-report}

1. Wählen Sie unter „Marketing-Aktivitäten“ das Programm aus, in dem Ihre **[!UICONTROL iOS]**- und **[!UICONTROL Android]**-Smart-Listen gespeichert sind.

   ![](assets/ten.png)

1. Wählen **[!UICONTROL unter]** die Option **[!UICONTROL Neues lokales Asset]** aus.

   ![](assets/eleven.png)

1. Klicken Sie auf **[!UICONTROL Bericht]**.

   ![](assets/twelve.png)

1. Setzen Sie den Typ auf **[!UICONTROL People Performance]**.

   ![](assets/thirteen.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/fourteen.png)

   Du machst das großartig! Fahren Sie nun mit dem nächsten Abschnitt fort.

## Mobile Smart-Listen als Spalten hinzufügen {#add-mobile-smart-lists-as-columns}

1. Klicken Sie im soeben erstellten Bericht auf **[!UICONTROL Setup]** und ziehen Sie dann **[!UICONTROL Benutzerdefinierte Spalten]** in die Arbeitsfläche.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Standardmäßig werden für den Bericht „Personen-Performance“ die letzten 7 Tage berücksichtigt. Sie können den Zeitrahmen ändern, indem Sie darauf doppelklicken.

1. Suchen Sie die zuvor erstellten Smart-Listen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/sixteen.png)

1. Klicken Sie **[!UICONTROL Bericht]**, um den Bericht auszuführen und Ihre Daten anzuzeigen.

   ![](assets/seventeen.png)

   Ziemlich cool, oder? Gut gemacht!
