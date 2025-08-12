---
solution: Marketo Engage
product: marketo
title: TITEL
description: Erfahren Sie, wie Sie die E-Mail-Erstellung mit wiederverwendbaren Designs und Modulen optimieren können, um Konsistenz und Effizienz im Design sicherzustellen.
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 1cfb28f47ba3c168292b298e1fc7ab2ff638b412
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 74%

---

# Anwenden von Designs auf Ihren E-Mail-Inhalt {#apply-email-themes}

>[!AVAILABILITY]
>
>Diese Funktion befindet sich derzeit in der Beta-Version und steht nur der Beta-Kundschaft zur Verfügung. Wenden Sie sich an den Adobe-Support, um am Beta-Programm teilzunehmen.

Mit Designs können technisch nicht versierte Benutzende wiederverwendbare Inhalte erstellen, die zu einer bestimmten Marke und Designsprache passen, indem sie zusätzlich zu den Standardvorlagen benutzerdefinierte Stile hinzufügen<!-- to achieve brand specific results-->.

Diese Funktion ermöglicht es Marketing-Fachleuten, visuell ansprechende, markenkonsistente E-Mails schneller und mit weniger Aufwand zu nutzen und gleichzeitig erweiterte Anpassungsoptionen für individuelle Design-Anforderungen bereitzustellen.

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## Schutzmechanismen und Einschränkungen {#themes-guardrails}

* Wenn Sie eine E-Mail von Grund auf neu erstellen, können Sie die Erstellung Ihres Inhalts mit einem Design beginnen, um schnell einen bestimmten Stil anzuwenden, der zu Ihrer Marke und Ihrem Design passt.

  Wenn Sie den Modus _Manuelle Formatierung_ wählen, können Sie keine Designs anwenden, es sei denn, Sie setzen Ihre E-Mail zurück.

* [Fragmente](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) sind zwischen den Modi _Verwenden von Designs_ und _Manueller Stil_ nicht kreuzkompatibel.

  Um ein Fragment in einem Inhalt verwenden zu können, auf den ein Design angewendet wird, muss dieses Fragment im Modus _Verwenden von Designs_ erstellt werden.

* Wenn Sie in HTML erstellte Inhalte verwenden, befinden Sie sich im [Kompatibilitätsmodus](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) und können keine Designs auf diese Inhalte anwenden.

  Um alle Funktionen der E-Mail-Designer, einschließlich Designs, vollständig zu nutzen, müssen Sie entweder neue Inhalte im _Verwenden von Designs_ erstellen oder Ihre [importierten HTML-Inhalte](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) konvertieren.

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## Erstellen eines Designs {#create-and-edit-themes}

Gehen Sie wie folgt vor, um ein Design zu definieren, das Sie in künftigen E-Mail-Inhalten nutzen können.

1. Erstellen Sie zunächst eine neue [E-Mail-Vorlage](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template).

1. Wählen Sie die Option **[!UICONTROL Designs erstellen oder bearbeiten]** aus.

   `![](assets/theme-create.png)`

1. Sie können entweder das Standarddesign auswählen oder eine Adobe- oder benutzerdefinierte Vorlage verwenden. Wählen Sie in diesem Beispiel das Standarddesign aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   `![](assets/theme-select.png)`

1. Beginnen Sie auf der Registerkarte **[!UICONTROL Allgemeine Einstellungen]** mit der Definition Ihres Designs, indem Sie ihm einen bestimmten Namen für Ihre Marke geben. Sie können die Standardbreite für Ihre E-Mails anpassen und auch das aktuelle Design exportieren, um es über Sandboxes hinweg freizugeben.

   `<!--![](assets/theme-general-settings.png)-->`

1. Verwenden Sie die Leiste auf der rechten Seite, um durch die verschiedenen Registerkarten zu navigieren und Ihre Designeinstellungen zu aktualisieren.

   `![](assets/theme-right-pane.png)`

1. Führen Sie folgende Schritte auf der Registerkarte **[!UICONTROL Farben]** aus:

   * Verwenden Sie die Schaltfläche **[!UICONTROL Bearbeiten]**, um eine **[!UICONTROL Farbpalette]** mit Standardfarben für Ihre Marke einzurichten. Wählen Sie eine **[!UICONTROL Voreinstellung]** aus, um schnell ein Farbschema zu erstellen oder jede Farbe Ihres Designs individuell anzupassen. Sie können auch eine Kombination aus beidem verwenden.

     `![](assets/theme-colors.gif)`

   * Klicken Sie auf **[!UICONTROL Variante hinzufügen]**, um mehrere Farbvarianten zu erstellen, z. B. den hellen und dunklen Modus, wobei jede Variante über eine eigene Farbpalette und Steuerelemente für Nuancen verfügt.

     `![](assets/theme-colors-variant.png)`

   * Klicken Sie für jede Variante auf das Symbol „Bearbeiten“, um ein einzelnes Element zu bearbeiten. Sie können die von Ihnen erstellte Standardpalette oder beliebige benutzerdefinierte Farben verwenden.

     `![](assets/theme-colors-edit-variant.gif)`

1. In den **[!UICONTROL Texteinstellungen]** können Sie die globale Schriftart festlegen, die Sie für Ihr gesamtes Design verwenden möchten. Für eine detailliertere Steuerung können Sie auch jede Überschrift und jeden Absatztyp bearbeiten, um die Schriftart, die Größe, den Stil usw. anzupassen.

   `![](assets/theme-text.png)`

1. Wählen Sie auf der Registerkarte **[!UICONTROL Abstand]** ein einzelnes Element aus der Liste aus, um es mit dem richtigen Abstand zwischen den verschiedenen Komponenten einzufügen.

   `<!--![](assets/theme-spacing.png)-->`

1. Mit den anderen Registerkarten auf der rechten Seite können Sie jedes Schaltflächenelement, jede Trennlinie, zusätzliche Bildformatierungen und den Abstand des Raster-Layouts für dieses Design separat verwalten.

   `<!--![](assets/theme-buttons.png)-->`

1. Klicken Sie auf **[!UICONTROL Speichern]**, um dieses Design für die zukünftige Verwendung zu speichern.

## Anwenden von Designs auf eine E-Mail {#apply-themes}

Gehen Sie wie folgt vor, um standardmäßige oder benutzerdefinierte Stil-Designs auf eine E-Mail anzuwenden.

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. Sie können eine der folgenden Aktionen auswählen:

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >Wenn Sie den Modus _Manuelle Formatierung_ wählen, können Sie keine Designs anwenden, es sei denn, Sie setzen Ihre E-Mail zurück.
     >
     >Um ein [Fragment](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) im Modus _Verwenden von Designs_ zu verwenden, muss dieses Fragment selbst im Modus _Verwenden von Designs_ erstellt worden sein.

1. Klicken Sie im E-Mail-Designer in der rechten Leiste auf die Schaltfläche **[!UICONTROL Designs]**. Es wird das Standard-Design oder das Design der Vorlage angezeigt. Sie können zwischen den beiden Farbvarianten für dieses Design wechseln.

   `![](assets/theme-default-hero.png)`

1. Klicken Sie auf den Pfeil neben dem aktuell verwendeten Design. Die Liste der verfügbaren benutzerdefinierten und Adobe-Designs wird angezeigt.

   `![](assets/theme-hero-change.png)`

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Designs]** und wählen Sie das von Ihnen erstellte Design aus.

   `![](assets/theme-select-custom.png)`

1. Klicken Sie auf einen Bereich außerhalb der Dropdown-Liste. Das neu ausgewählte benutzerdefinierte Design wendet seine Stile automatisch auf alle E-Mail-Komponenten an. Sie können zwischen den beiden Farbvarianten wechseln.

1. Wenn eine Komponente ausgewählt wird, können Sie ihren Stil immer noch über das entsprechende Symbol entsperren.

   `![](assets/theme-unlock-style.png)`

Sie können jederzeit zwischen Designs wechseln. Der E-Mail-Inhalt bleibt unverändert, aber die Stile werden aktualisiert, um das neue Design widerzuspiegeln.

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
