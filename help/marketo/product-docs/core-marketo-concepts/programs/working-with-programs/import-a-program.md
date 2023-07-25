---
unique-page-id: 1147108
description: Programm importieren - Marketo-Dokumente - Produktdokumentation
title: Programm importieren
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Programm importieren {#import-a-program}

Ein Programm kann aus einem Marketo-Abonnement in ein anderes importiert werden. Sie können beispielsweise ein Programm in einer Sandbox erstellen und es dann in Ihr Live-Abonnement importieren. Außerdem können Sie ein vordefiniertes Programm aus der Marketo-Programmbibliothek importieren.

## Programm importieren {#importing-a-program}

1. Navigieren Sie zu **Marketingaktivitäten.**

   ![](assets/import-a-program-1.png)

1. Klicken **Neu** angezeigt. Auswählen **Importprogramm**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >Der Programm-Import ist nur für Benutzer verfügbar, deren Rollen mit der Berechtigung Programm importieren aktiviert sind. Weitere Informationen [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Um ein Sandbox-Konto mit Ihrem Live-Abonnement zu verbinden, wenden Sie sich an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Marketo auswählen **Abonnement** und ein Importprogramm. Klicken **Nächste**.

   ![](assets/import-a-program-3.png)

1. Geben Sie eine **Kampagnenordner** für das importierte Programm. Klicken **Weiter.**

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Stellen Sie sicher **Standardkonflikt verwenden** -Regeln ausgewählt ist. Konfliktregeln sind erforderlich, wenn Sie Programme in eine Instanz importieren, die Assets mit demselben Namen enthält.

1. Wählen Sie die gewünschten Konfliktdetails aus und klicken Sie auf **Nächste**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Beim Importieren eines Programms, das Custom Flow-Schritte oder Smart List-Regeln verwendet, die von einem Flow Step Service in eine Zielinstanz abgeleitet werden, in der mehr als ein kompatibler Service Provider vorhanden ist, wird der importierende Benutzer aufgefordert, dem richtigen Service Provider in der Zielinstanz Schritte oder Regeln zuzuweisen.

1. Details in der Vorschau anzeigen und **Import** das Programm.

   ![](assets/import-a-program-6.png)

Sie erhalten eine E-Mail-Bestätigung, sobald der Import abgeschlossen ist.

>[!NOTE]
>
>Sie müssen importierte Batch-Kampagnen neu planen und Trigger-Kampagnen aktivieren. Das System deaktiviert automatisch Kampagnenzeitpläne und Trigger-Kampagnen im importierten Programm.

## Auswirkungen auf externe Assets bei Programmeinfuhren {#impact-on-external-assets-during-program-imports}

Programme verwenden externe Assets wie E-Mail-Vorlagen, Landingpage-Vorlagen, Bilder, Formulare, Token und Programm-Tags. Sie können konfigurieren, wie Landingpage-Vorlagen und Programm-Tags verarbeitet werden, und Marketo verwaltet den Rest automatisch.

**E-Mail-/Landingpage-Vorlagen:** E-Mail-/Landingpage-Vorlagen werden in Design Studio importiert. Sie können Konfliktregeln verwenden, um das Verhalten zu konfigurieren, wenn eine Vorlage mit demselben Namen vorhanden ist. Unter Verwendung der Standardregel wird eine Zahl an eine Vorlage angehängt, wenn eine mit demselben Namen vorhanden ist. Wenn Sie beispielsweise bereits über eine Vorlage mit dem Namen &quot;Standardvorlage&quot;verfügen, erhält die neue Vorlage den Namen &quot;Standardvorlage - 1&quot;.

**Landing Pages/Forms:** Wenn ein Formular oder eine Landingpage mit demselben Namen in Design Studio vorhanden ist, werden sie dennoch importiert, jedoch mit einer Nummer, die an ihren Namen angehängt wird (z. B.: Landingpage - 1).

**Bilder:** Bilder, die von Landingpages verwendet werden, werden in das Design-Studio importiert, es sei denn, es existiert eines mit demselben Namen.

**Token:** Token, die außerhalb eines Programms liegen, werden während des Importvorgangs in lokale Token konvertiert.

>[!CAUTION]
>
>Bildtyp Meine Token werden für Programmimporte nicht unterstützt. Wenn ein Programm mit Bildtyp meine Token importiert wird, **no** Token werden durchkommen.

**Programm-Tags:** Sie können Konfliktregeln verwenden, um zu steuern, wie Programm-Tags behandelt werden, die im Zielkonto nicht vorhanden sind. Durch die Verwendung der Standardregel werden die Programm-Tags erstellt, oder Sie können die Tags ignorieren.

>[!CAUTION]
>
>Beim Importieren eines Programms werden E-Mails/Landingpages mit [dynamischer Inhalt](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) werden übersprungen.
