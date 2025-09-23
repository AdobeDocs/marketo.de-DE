---
unique-page-id: 1147108
description: Programm importieren - Marketo-Dokumente - Produktdokumentation
title: Importieren eines Programms
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 1%

---

# Importieren eines Programms {#import-a-program}

Ein Programm kann von einem Marketo Engage-Abonnement in ein anderes importiert werden. Sie können beispielsweise ein Programm in einer Sandbox erstellen und es dann in Ihr Live-Abonnement importieren. Sie können auch ein vordefiniertes Programm aus der [Marketo-Programmbibliothek importieren](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>Bei Programmen mit Smart Lists, die den Trigger „Benutzerdefiniertes Objekt wird aktualisiert“ enthalten, schlägt der Import fehl. Entfernen Sie diesen Trigger aus allen Smart Lists, bevor Sie die unten beschriebenen Schritte ausführen.

## Programm importieren {#importing-a-program}

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/import-a-program-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Programm importieren]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* Programm-Import ist nur für Benutzer verfügbar, die Rollen mit aktivierter Berechtigung „Programm importieren“ haben. Weitere Informationen zu [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Um ein Sandbox-Konto mit Ihrem Live-Abonnement zu verbinden, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Wählen Sie ein Marketo **[!UICONTROL Abonnement]** und ein zu importierendes Programm aus. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-3.png)

1. Geben Sie **[!UICONTROL importierten Programm einen]** Kampagnenordner“ an. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Stellen Sie sicher **[!UICONTROL dass „Standardkonfliktregeln verwenden]** ausgewählt ist. Konfliktregeln sind erforderlich, wenn Sie Programme in eine Instanz mit Assets desselben Namens importieren.

1. Wählen Sie die gewünschten Konfliktdetails aus und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Beim Importieren eines Programms, das benutzerdefinierte Flussschritte oder Regeln für die Smart-Liste verwendet, die von einem Flow Step-Service abgeleitet sind, in eine Zielinstanz, in der mehr als ein kompatibler Service Provider vorhanden ist, wird der importierende Benutzer aufgefordert, dem richtigen Service Provider in der Zielinstanz Schritte oder Regeln zuzuweisen.

1. Vorschau von Details und **[!UICONTROL Import]** des Programms.

   ![](assets/import-a-program-6.png)

Sie erhalten eine E-Mail-Bestätigung, sobald der Import abgeschlossen ist.

>[!NOTE]
>
>Sie müssen importierte Batch-Kampagnen neu planen und Trigger-Kampagnen aktivieren. Das System deaktiviert automatisch Kampagnenpläne und Trigger-Kampagnen im importierten Programm.

## Auswirkungen auf externe Assets während der Programmimporte {#impact-on-external-assets-during-program-imports}

Programme verwenden externe Assets wie E-Mail-Vorlagen, Landingpage-Vorlagen, Bilder, Formulare, Token und Programm-Tags. Sie können konfigurieren, wie Landingpage-Vorlagen und Programm-Tags verarbeitet werden. Marketo verwaltet den Rest automatisch.

**E-Mail-/Landingpage-Vorlagen:** E-Mail-/Landingpage-Vorlagen werden in Design Studio importiert. Sie können Konfliktregeln verwenden, um das Verhalten zu konfigurieren, wenn eine Vorlage mit demselben Namen vorhanden ist. Unter Verwendung der Standardregel wird eine Zahl an eine Vorlage angehängt, wenn eine mit demselben Namen vorhanden ist. Wenn Sie beispielsweise bereits über eine Vorlage mit dem Namen „Standardvorlage“ verfügen, erhält die neue den Namen „Standardvorlage - 1“.

**Landingpages/Forms:** Wenn in Design Studio ein Formular oder eine Landingpage mit demselben Namen vorhanden ist, werden sie weiterhin importiert, jedoch mit einer an den Namen angehängten Nummer (z. B.: Landingpage - 1).

**Bilder:** von Landingpages verwendeten Bilder werden in das Design-Studio importiert, es sei denn, es ist bereits ein Bild mit demselben Namen vorhanden.

**Token:** Token, die außerhalb eines Programms leben, werden während des Importvorgangs in lokale Token konvertiert.

>[!CAUTION]
>
>Bildtyp Meine Token werden für Programmimporte nicht unterstützt. Wenn ein Programm mit dem Bildtyp Meine Token importiert wird, werden _keine_ Token angezeigt.

**Programm-Tags:** Sie können Konfliktregeln verwenden, um zu steuern, wie Programm-Tags, die nicht im Zielkonto vorhanden sind, behandelt werden. Wenn Sie die Standardregel verwenden, werden die Programm-Tags erstellt. Sie können aber auch wählen, ob Sie die Tags ignorieren möchten.

>[!CAUTION]
>
>Beim Importieren eines Programms werden E-Mails/Landingpages mit [dynamischen ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"}) übersprungen.
