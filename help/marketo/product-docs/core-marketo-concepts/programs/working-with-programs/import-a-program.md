---
unique-page-id: 1147108
description: Programm importieren - Marketo-Dokumente - Produktdokumentation
title: Programm importieren
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Programm importieren {#import-a-program}

Ein Programm kann von einem Marketo Engage-Abonnement in ein anderes importiert werden. Sie können beispielsweise ein Programm in einer Sandbox erstellen und es dann in Ihr Live-Abonnement importieren. Außerdem können Sie ein vordefiniertes Programm aus der [Marketo-Programmbibliothek](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"} importieren.

>[!CAUTION]
>
>Bei Programmen mit Smart-Listen, die den Trigger &quot;Benutzerdefiniertes Objekt wird aktualisiert&quot;enthalten, schlägt der Import fehl. Entfernen Sie diesen Trigger aus allen Smart-Listen, bevor Sie die unten beschriebenen Schritte ausführen.

## Programm importieren {#importing-a-program}

1. Wechseln Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/import-a-program-1.png)

1. Klicken Sie auf die Dropdownliste **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Programm importieren]** aus.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* Der Programm-Import ist nur für Benutzer verfügbar, deren Rollen mit der Berechtigung Programm importieren aktiviert sind. Erfahren Sie mehr über [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}, um ein Sandbox-Konto mit Ihrem Live-Abonnement zu verbinden.

1. Wählen Sie eine Marketo **[!UICONTROL Subscription]** und ein zu importierendes Programm aus. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-3.png)

1. Geben Sie einen **[!UICONTROL Kampagnenordner]** für das importierte Programm an. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass **[!UICONTROL Standardkonfliktregeln verwenden]** ausgewählt ist. Konfliktregeln sind erforderlich, wenn Sie Programme in eine Instanz importieren, die Assets mit demselben Namen enthält.

1. Wählen Sie die gewünschten Konfliktdetails aus und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Beim Importieren eines Programms, das Custom Flow-Schritte oder Smart List-Regeln verwendet, die von einem Flow Step Service in eine Zielinstanz abgeleitet werden, in der mehr als ein kompatibler Service Provider vorhanden ist, wird der importierende Benutzer aufgefordert, dem richtigen Service Provider in der Zielinstanz Schritte oder Regeln zuzuweisen.

1. Vorschaudetails und **[!UICONTROL Importieren]** des Programms anzeigen.

   ![](assets/import-a-program-6.png)

Sie erhalten eine E-Mail-Bestätigung, sobald der Import abgeschlossen ist.

>[!NOTE]
>
>Sie müssen importierte Batch-Kampagnen neu planen und Trigger-Kampagnen aktivieren. Das System deaktiviert automatisch Kampagnenzeitpläne und Trigger-Kampagnen im importierten Programm.

## Auswirkungen auf die externe Assets bei Programmeinfuhren {#impact-on-external-assets-during-program-imports}

Programme verwenden externe Assets wie E-Mail-Vorlagen, Landingpage-Vorlagen, Bilder, Formulare, Token und Programm-Tags. Sie können konfigurieren, wie Landingpage-Vorlagen und Programm-Tags verarbeitet werden, und Marketo verwaltet den Rest automatisch.

**E-Mail-/Landingpage-Vorlagen:** E-Mail-/Landingpage-Vorlagen werden in Design Studio importiert. Sie können Konfliktregeln verwenden, um das Verhalten zu konfigurieren, wenn eine Vorlage mit demselben Namen vorhanden ist. Unter Verwendung der Standardregel wird eine Zahl an eine Vorlage angehängt, wenn eine mit demselben Namen vorhanden ist. Wenn Sie beispielsweise bereits über eine Vorlage mit dem Namen &quot;Standardvorlage&quot;verfügen, erhält die neue Vorlage den Namen &quot;Standardvorlage - 1&quot;.

**Landingpages/Forms:** Wenn ein Formular oder eine Landingpage mit demselben Namen in Design Studio vorhanden ist, werden sie dennoch importiert, wobei eine Nummer an ihren Namen angehängt wird (z. B.: Landingpage - 1).

**Bilder:** Von Landingpages verwendete Bilder werden in das Design-Studio importiert, es sei denn, es existiert eines mit demselben Namen.

**Token:** Token, die außerhalb eines Programms liegen, werden während des Importvorgangs in lokale Token konvertiert.

>[!CAUTION]
>
>Bildtyp Meine Token werden für Programmimporte nicht unterstützt. Wenn ein Programm importiert wird, das über den Bildtyp meiner Token verfügt, werden _no_-Token angezeigt.

**Programm-Tags:** Sie können Konfliktregeln verwenden, um zu steuern, wie Programm-Tags, die nicht im Zielkonto vorhanden sind, behandelt werden. Durch die Verwendung der Standardregel werden die Programm-Tags erstellt, oder Sie können die Tags ignorieren.

>[!CAUTION]
>
>Beim Importieren eines Programms werden E-Mails/Landingpages mit [dynamischem Inhalt](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} übersprungen.
