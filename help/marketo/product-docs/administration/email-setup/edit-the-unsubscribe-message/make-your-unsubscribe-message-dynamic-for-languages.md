---
unique-page-id: 6848782
description: Dynamische Abmeldemeldung für Sprachen - Marketo-Dokumente - Produktdokumentation
title: Dynamische Abmeldemeldung für Sprachen
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 3%

---

# Dynamische Abmeldemeldung für Sprachen {#make-your-unsubscribe-message-dynamic-for-languages}

Die Standard-Abmelde-Nachricht und der entsprechende Link sind auf Englisch verfügbar. Sie können dynamische Inhalte verwenden, um sie in verschiedenen Sprachen anzuzeigen.

>[!NOTE]
>
>Dieser Artikel stellt eine Best Practice dar, kann aber auf andere Weise durchgeführt werden.

## Daten vorbereiten {#prepare-your-data}

1. [Erstellen Sie ein benutzerdefiniertes Feld ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) mit dem Namen &quot;Bevorzugte Sprache&quot;. (Richten Sie es in Ihrem CRM ein, wenn dieses Feld synchronisiert werden soll).

   >[!TIP]
   >
   >Verwenden Sie dieses Feld zukünftig, wenn Sie [ein Formular ](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) erstellen, um die Spracheinstellung zu erfassen.

## Segmentierung erstellen {#create-segmentation}

1. Wechseln Sie zur **[!UICONTROL Datenbank]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. Klicken Sie in der Dropdown-Liste **[!UICONTROL Neu]** auf **[!UICONTROL Neue Segmentierung]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Benennen Sie die Segmentierung mit &quot;**[!UICONTROL Bevorzugte Sprache]**&quot;. Klicken Sie auf **[!UICONTROL Segment hinzufügen]**. Geben Sie eine Sprache ein.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Das Standardsegment ist Englisch.

1. Fügen Sie weiterhin Segmente hinzu, bis alle Ihre Sprachen repräsentiert sind. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Segment auswählen.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Gehen Sie zur Registerkarte **[!UICONTROL Smart List]** . Geben Sie **[!UICONTROL Bevorzugte Sprache]** in das Suchfeld ein. Ziehen Sie den Filter auf die Arbeitsfläche.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Legen Sie die entsprechende Sprache fest.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Wiederholen Sie diese Schritte für alle Ihre Sprachen. Wählen Sie dann das Dropdown-Menü **[!UICONTROL Segmentierungsaktionen]** aus und klicken Sie auf **[!UICONTROL Genehmigen]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Snippet erstellen {#create-a-snippet}

1. Wechseln Sie zu **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. Klicken Sie im Dropdown-Menü **[!UICONTROL Neu]** auf **[!UICONTROL Neues Snippet]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Nennen Sie das Snippet &quot;**Unsubscribe Message**&quot;. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Geben Sie Ihre standardmäßige Abmelde-Nachricht ein, markieren Sie sie und klicken Sie auf das Hyperlink-Symbol.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Kopieren Sie dieses Token: `{{system.unsubscribeLink}}` und fügen Sie es in das Feld **[!UICONTROL URL]** ein. Klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Wählen Sie **[!UICONTROL Segment nach]** im Abschnitt **[!UICONTROL Segmentierung]** aus.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Geben Sie in der Dropdown-Liste **[!UICONTROL Segmentierung]** den Wert **[!UICONTROL Bevorzugt]** ein und wählen Sie **[!UICONTROL Bevorzugte Sprache]** aus. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Wählen Sie ein Segment aus der Baumstruktur aus. Klicken Sie auf Ihre Abmeldung und dann auf das Link-Symbol.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Stellen Sie sicher, dass `{{system.unsubscribeLink}}` noch im Feld **[!UICONTROL URL]** enthalten ist. Bearbeiten Sie den **[!UICONTROL Text anzeigen]** entsprechend der ausgewählten Sprache. Klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Wiederholen Sie diese Schritte für alle Ihre Segmente. Gehen Sie dann zurück zu **[!UICONTROL Design Studio]**, klicken Sie auf die Dropdown-Liste **[!UICONTROL Ausschnitt-Aktionen]** und klicken Sie auf **[!UICONTROL Genehmigen]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Fantastisch. Fast da!

## Snippet in einer E-Mail verwenden {#use-snippet-in-an-email}

1. Klicken Sie im E-Mail-Editor auf das bearbeitbare Element. Klicken Sie dann auf das Zahnradsymbol und wählen Sie **[!UICONTROL Durch Snippet ersetzen]** aus. Wenn Sie ein bearbeitbares Snippet-Element auswählen, klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Suchen und wählen Sie Ihr Snippet aus der Dropdown-Liste aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Klicken Sie zum Testen auf **[!UICONTROL Zurück]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ... dann die Registerkarte **[!UICONTROL Dynamisch]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Klicken Sie auf die verschiedenen Sprachen, um die Änderung des Snippets anzuzeigen.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Natürlich können Sie den Rest Ihrer E-Mail auch für dynamische Sprachen bearbeiten. Führen Sie auf der Abmeldeseite die gleiche Technik aus, während Sie damit fertig sind.

## Anpassen der Abmeldeseite mit dynamischen Inhalten {#customizing-your-unsubscribe-page-with-dynamic-content}

Wenn Sie möchten, dass Ihre Personen zu einer Abmeldeseite in der gewünschten Sprache gelangen, können Sie dynamischen Inhalt auf der Landingpage und der Bestätigungsseite verwenden.

1. Navigieren Sie zu **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Geben Sie _Unsubscribe_ in das Suchfeld ein und wählen Sie die gewünschte Abmeldeseite aus.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Wählen Sie **[!UICONTROL Segment nach]** aus.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Suchen Sie das Segment **[!UICONTROL Bevorzugte Sprache]** . Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Bearbeiten Sie den Inhalt für jede Landingpage, validieren Sie, und Sie können loslegen!

   >[!NOTE]
   >
   >Erfahren Sie mehr über [dynamischen Inhalt](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) und alle coolen Dinge, die Sie tun können.
