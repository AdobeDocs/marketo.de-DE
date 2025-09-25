---
description: Dunkelmodus - Marketo-Dokumente - Produktdokumentation
title: Dunkler Modus
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: e6aa9e921776ca635c4c234b950c173bc000a3f7
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 62%

---

# Dunkler Modus {#dark-mode}

Beim Entwerfen Ihrer E-Mails können Sie mit der E-Mail-Designer zur Ansicht **[!UICONTROL Dunkelmodus]** wechseln.

Im **[!UICONTROL Dunkelmodus]** können Sie bestimmte benutzerdefinierte Einstellungen definieren, die angezeigt werden sollen, indem Sie E-Mail-Clients unterstützen, wenn ihr Dunkelmodus aktiviert ist.

## Was ist der dunkle Modus? {#what-is-dark-mode}

Der Dunkelmodus ermöglicht es unterstützenden E-Mail-Clients und -Programmen, E-Mails mit dunkleren Hintergründen und helleren Farben für Text, Schaltflächen und andere Benutzeroberflächenelemente anzuzeigen. Dadurch werden die Augen entlastet, die Akkulaufzeit verkürzt und die Lesbarkeit in schwach beleuchteten Umgebungen verbessert, sodass das Betrachten angenehmer wird.

## Schutzmechanismen {#guardrails}

Das Dark-Mode-Rendering kann in verschiedenen E-Mail-Clients erheblich variieren.

Bevor Sie den Dunkelmodus verwenden, müssen Sie wissen, wie die wichtigsten E-Mail-Clients damit umgehen. Es gibt drei Fälle, in denen unterschieden werden muss:

### Clients unterstützen keinen Dunkelmodus {#not-supporting}

Einige E-Mail-Clients unterstützen diese Funktion überhaupt nicht, z. B.:

* Yahoo!Mail
* AOL

Unabhängig davon, ob Sie benutzerdefinierte Einstellungen für den Dunkelmodus definieren oder nicht, zeigen diese E-Mail-Clients nie Rendering im Dunkelmodus an.

### Clients, die ihren eigenen Dunkelmodus anwenden {#default-support}

Einige E-Mail-Clients wenden systematisch ihren eigenen standardmäßigen Dunkelmodus auf alle empfangenen E-Mails an. Farben, Hintergründe, Bilder usw. werden automatisch mit den für diesen E-Mail-Client spezifischen Einstellungen für den Dunkelmodus angepasst. Externe Änderungen sind nicht möglich.

Diese Clients zum Beispiel:

* Gmail (Desktop-Webmail, iOS, Android, Mobile-Webmail)
* Outlook Windows
* Outlook Windows Mail

Wenn Sie in diesem Fall benutzerdefinierte Einstellungen für den Dunkelmodus in der E-Mail-Designer definieren, werden diese Einstellungen durch die E-Mail-Client-Einstellungen überschrieben.

Während diese E-Mail-Clients also den Dunkelmodus verarbeiten, wird Ihr spezifisches Dunkelmodus-Design nicht gerendert.

### Clients, die den benutzerdefinierten Dunkelmodus unterstützen {#custom-support}

Andere E-Mail-Clients bieten die Option, den benutzerdefinierten Dunkelmodus mit der `@media (prefers-color-scheme: dark)`-Abfrage zu rendern, was die von der [!DNL Marketo Engage] E-Mail-Designer verwendete Methode ist.

Im Folgenden finden Sie eine Liste der wichtigsten Clients, die diese Option handhaben:

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

In diesem Fall sollten die Einstellungen angezeigt werden, die Sie in der E-Mail-Designer definieren.

>[!NOTE]
>
>In diesem Abschnitt erfahren Sie, wie Sie mit der E-Mail-Designer benutzerdefinierte Einstellungen für [ Dunkelmodus ](#define-custom-dark-mode).

Je nach E-Mail-Client können jedoch einige Einschränkungen gelten. Beispielsweise erzeugen einige Clients wie Apple Mail 16 (macOs 13) keinen Dunkelmodus, wenn Bilder vorhanden sind.

Um optimale Ergebnisse zu erzielen, testen Sie Ihren Inhalt in den E-Mail-Clients, auf die Sie abzielen. Um eine Simulation anzuzeigen, die dem Endergebnis für jeden Client so nahe wie möglich kommt, verwenden Sie die Funktion [E-Mail-Rendering](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) in der E-Mail-Designer.

## Dunkler Modus im E-Mail-Designer {#dark-mode-email-designer}

Beim dunklen Modus im E-Mail-Designer sind zwei Aspekte zu berücksichtigen:

* Sie können eine Vorschau anzeigen, wie der standardmäßige dunkle Modus in den meisten unterstützenden E-Mail-Clients gerendert wird. [Weitere Informationen](#preview-dark-mode)

* Wenn Sie die Standardeinstellungen unterstützender E-Mail-Clients überschreiben möchten, können Sie benutzerdefinierte Einstellungen für den Dunkelmodus in der E-Mail definieren, die Sie bearbeiten. [Weitere Informationen](#define-custom-dark-mode)

### Vorschau des standardmäßigen dunklen Modus {#preview-dark-mode}

Gehen Sie wie folgt vor, um auf den dunklen Modus im E-Mail-Designer zuzugreifen und eine Vorschau der Einstellungen für den standardmäßigen dunklen Modus zu erhalten.

1. Wählen Sie auf der Startseite des E-Mail-Designers die Option **[!UICONTROL Erstellen von neuen Inhalten]** aus.

1. Fügen Sie [Strukturen und Inhalte](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content) zu Ihrer E-Mail hinzu.

1. Aktivieren Sie oben rechts den Umschalter **[!UICONTROL Dunkelmodus]**.

   SCREENSHOT

1. Die Vorschau des standardmäßigen dunklen Modus wird angezeigt.

   SCREENSHOT

Standardmäßig wendet die Vorschau des dunklen Modus im E-Mail-Designer das Farbschema „Vollfarbinvertierung“ auf alle Elemente außer auf Bilder und Symbole an. 

Das bedeutet, dass Bereiche mit hellen und dunklen Elementen erkannt und invertiert werden, sodass helle Hintergründe dunkel und dunkler Text hell werden, während dunkle Hintergründe hell und heller Text dunkel werden.

>[!CAUTION]
>
>Das endgültige Rendering kann je nach E-Mail-Client der Empfängerinnen und Empfänger variieren. Um für jeden E-Mail-Client eine Simulation anzuzeigen, die dem Endergebnis möglichst nahe kommt, verwenden Sie die Option [E-Mail-Rendering](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

### Definieren des benutzerdefinierten dunklen Modus {#define-custom-dark-mode}

Nach dem Wechsel in den **[!UICONTROL dunklen Modus]** können Sie bestimmte Stilelemente Ihres Inhalts bearbeiten, die nur angezeigt werden, wenn der dunkle Modus im E-Mail-Client der Empfängerin bzw. des Empfängers aktiviert ist, sofern diese Funktion unterstützt wird.

>[!WARNING]
>
>Das endgültige Rendering im dunklen Modus hängt vom individuellen E-Mail-Client ab, die Ergebnisse können daher variieren. [Weitere Informationen](#guardrails)

Um die benutzerdefinierten Dunkelmodus-Stile von E-Mail-Designer zu nutzen, verwendet Journey Optimizer die `@media (prefers-color-scheme: dark)` CSS-Abfrage , die erkennt, ob der E-Mail-Client der Benutzenden auf den Dunkelmodus eingestellt ist, und das in Ihrer E-Mail definierte Design mit dunklem Design anwendet.

Gehen Sie wie folgt vor, um die Einstellungen für den benutzerdefinierten dunklen Modus zu definieren.

1. Stellen Sie sicher, dass Sie im E-Mail-Designer in den **[!UICONTROL Dunklen Modus]** wechseln. [Weitere Informationen](#preview-dark-mode)

1. Bearbeiten Sie alle Stilattribute wie Text, Hintergrund, Schaltflächen usw.

1. Sie können die Farben von Bildern und Symbolen nicht ändern, Sie können jedoch bestimmte Assets nur für den dunklen Modus definieren. Wählen Sie dazu ein Bild aus. Wechseln Sie über den entsprechenden Umschalter im Bereich **[!UICONTROL Einstellungen]** zu **[!UICONTROL Dunkler Modus]** und wählen Sie ein anderes Asset aus.

   SCREENSHOT

1. Sie können jederzeit die Option **[!UICONTROL Zur Live-Ansicht wechseln]** wählen, um zu überprüfen, wie Ihre Inhalte auf verschiedenen Gerätegrößen gerendert werden. Wählen Sie in dieser Ansicht den Umschalter für den dunklen Modus oben auf dem Bildschirm aus, um eine Vorschau der Version Ihres Inhalts im dunklen Modus auf den verschiedenen Geräten anzuzeigen.

   SCREENSHOT

   >[!CAUTION]
   >
   >Die Live-Ansicht ist eine allgemeine Vorschau, die vergleicht, wie das Rendering über verschiedene Gerätegrößen hinweg aussehen könnte. Das endgültige Rendering kann je nach E-Mail-Client der Empfängerinnen und Empfänger variieren.

1. Wenn Sie mit den Änderungen für den dunklen Modus zufrieden sind, klicken Sie auf **[!UICONTROL Inhalt simulieren]**.

   SCREENSHOT

1. Wählen Sie **[!UICONTROL E-Mail rendern]** und verbinden Sie sich mit Ihrem Litmus-Konto. Sie können das endgültige Rendering des dunklen Modus für verschiedene E-Mail-Clients sehen. Weitere Informationen zu [E-Mail-Rendering](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

   >[!WARNING]
   >
   >Auch wenn die Simulation dem Aussehen von E-Mails im dunklen Modus sehr nahe kommt, kann das tatsächliche Rendering aufgrund von Variationen bei E-Mail-Service-Anbietern oder Einstellungen auf Geräteebene unterschiedlich sein.

## Best Practices {#best-practices}

Da der dunkle Modus in den wichtigsten E-Mail-Clients immer beliebter wird, müssen Sie berücksichtigen, wie Ihre E-Mails in hellen und dunklen Umgebungen gerendert werden – unabhängig davon, ob Sie einen [benutzerdefinierten dunklen Modus](#define-custom-dark-mode) verwenden oder nicht.

Der dunkle Modus kann Farben, Hintergründe und Bilder verändern – und manchmal bestimmte Design-Entscheidungen überschreiben. Befolgen Sie die unten aufgeführten Best Practices, um visuelle Konsistenz, Barrierefreiheit und Markenintegrität sicherzustellen.

**Optimieren Ihrer Bilder und Logos**

* Speichern Sie Logos und Symbole als PNGs mit transparentem Hintergrund, um sichtbare weiße Felder im dunklen Modus zu vermeiden.

* Vermeiden Sie Bilder mit hartcodierten weißen oder hellen Hintergründen.

* Wenn Transparenz nicht möglich ist, platzieren Sie Bilder in Ihrem Design auf einem einfarbigen Hintergrund, um unangenehme Farbinversionen zu verhindern.

**Beachten Ihrer Hintergründe**

* Stellen Sie einen ausreichenden Kontrast zwischen Text- und Hintergrundfarben sicher, damit die Lesbarkeit sowohl im hellen als auch im dunklen Modus gewahrt bleibt.

* Vermeiden Sie es, sich bei kritischen Inhalten allein auf Hintergrundfarben zu verlassen. Einige Clients überschreiben Hintergrundfarben im dunklen Modus, sodass Sie sicherstellen müssen, dass wichtige Informationen weiterhin sichtbar sind.

**Entwerfen barrierefreier Inhalte im dunklen Modus**

* Verwenden Sie Farbkombinationen, die für Menschen mit Farbenblindheit leicht zu unterscheiden sind.

* Verwenden Sie eine Mitteltonpalette, um sowohl vor hellen als auch vor dunklen Hintergründen einen Kontrast sicherzustellen.

* Verwenden Sie barrierefreie Farbkombinationen mit hohem Kontrast, um die Lesbarkeit zu verbessern und die WCAG-Standards (Web Content Accessibility Guidelines) zu erfüllen. Verwenden Sie Tools wie die Kontrastprüfung von WebAIM, um den Farbkontrast zu überprüfen.

* Vermeiden Sie dünne Schriftarten, da sie die Lesbarkeit beeinträchtigen können. Wenn für Ihre Marke eine dünne Schriftart erforderlich ist, verwenden Sie sie für den dunklen Modus eine Fettformatierung.

* Vermeiden Sie reines Weiß auf reinem Schwarz, da dies die Augen belasten kann und von einigen E-Mail-Clients möglicherweise automatisch invertiert wird.

* Wenn der dunkle Modus nicht unterstützt wird, können Sie barrierefreie Fallback-Stile bereitstellen.

**Testen Ihrer E-Mails in einer Umgebung im dunklen Modus**

* Nutzen Sie die [Vorschau des dunklen Modus](#preview-dark-mode) im E-Mail-Designer. Diese verwendet invertierte Farbschemata, sodass Sie Probleme frühzeitig erkennen.

* Verwenden Sie die Option [E-Mail-Rendering](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md), die Litmus zur Simulation Ihrer Designs in wichtigen E-Mail-Clients (Apple Mail, Gmail, Outlook) nutzt, damit Sie sehen, wie sich Farben und Bilder im dunklen Modus verhalten.
