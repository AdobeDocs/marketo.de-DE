---
description: E-Mail-Authoring - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Authoring
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: af8afc9342a4ca0b4032c4d7c761703adb5a6701
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 4%

---

# E-Mail-Authoring {#email-authoring}

Erfahren Sie, wie Sie E-Mails in der neuen Marketo Engage E-Mail-Designer erstellen, personalisieren und in der Vorschau anzeigen.

>[!IMPORTANT]
>
>Dieser Artikel ist nur für Mitglieder der Beta-Version des neuen Marketo Engage-E-Mail-Editors gedacht. Bitte nicht verbreiten.

## Erstellen einer E-Mail {#create-an-email}

1. Melden Sie sich über die [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"} bei Marketo Engage an.

1. Wählen Sie in My Marketo **Design Studio** aus.

   ![](assets/create-an-email-1.png)

1. Wählen Sie im Baum **E-Mails (neuer Editor)** aus.

   ![](assets/create-an-email-2.png)

1. Klicken Sie auf die Schaltfläche **E-Mail erstellen** .

   ![](assets/create-an-email-3.png)

1. Geben Sie einen E-Mail-Namen und eine Betreffzeile ein. Klicken Sie auf **Erstellen**.

   ![](assets/create-an-email-4.png)

Das ist es. Jetzt ist es an der Zeit, Ihre E-Mail zu entwerfen.

## Inhaltstyp auswählen {#choose-your-content-type}

1. Klicken Sie in der soeben erstellten E-Mail auf **E-Mail-Inhalt hinzufügen**.

   ![](assets/choose-your-content-type-1.png)

1. Die Seite _E-Mail erstellen_ wird geladen. Sie können aus mehreren Optionen wählen:

* [Design von Grund auf neu](#design-from-scratch) mithilfe des visuellen E-Mail-Editors

* [Importieren Sie Ihre eigene HTML](#import-html) über eine HTML- oder ZIP-Datei

* [Wählen Sie eine vorhandene Vorlage aus](#choose-a-template) (einen unserer Beispiele oder einen bereits gespeicherten)

### Von Grund auf gestalten {#design-from-scratch}

Verwenden Sie beim Erstellen von neuen Texten im E-Mail-Editor die folgenden Optionen, um Ihren Inhalt zu definieren.

1. Wählen Sie auf der Seite _E-Mail erstellen_ die Option **Design von Grund auf neu** aus.

1. Fügen Sie [Struktur und Inhalt](#add-structure-and-content) zu Ihrer E-Mail hinzu.

1. Fügen Sie [Bilder](#add-assets) hinzu.

1. [Personalisieren](#personalize-content) Sie Ihren Inhalt.

1. Überprüfen Sie Links und [Bearbeiten-Tracking](#edit-url-tracking).

### Importieren von HTML {#import-html}

Sie können vorhandenen HTML-Inhalt importieren, um Ihre E-Mail zu erstellen. Der Inhalt kann wie folgt lauten:

* Eine HTML-Datei mit integriertem Stylesheet

* Eine ZIP-Datei mit einer HTML-Datei, dem Stylesheet (.css) und Bildern.

>[!NOTE]
>
>Die Dateistruktur des komprimierten Ordners ist freigestellt. Verweise müssen jedoch relativ sein und mit der Baumstruktur des ZIP-Ordners übereinstimmen.

1. Wählen Sie auf der Seite Vorlage erstellen die Option **HTML importieren** aus.

1. Ziehen Sie die gewünschte HTML- oder ZIP-Datei per Drag-and-Drop (oder wählen Sie eine Datei auf Ihrem Computer aus) und klicken Sie auf **Importieren**.

   ![](assets/authoring-import-your-html-1.png)

>[!NOTE]
>
>Wenn der HTML-Inhalt hochgeladen wird, befindet sich der Inhalt im Kompatibilitätsmodus. In diesem Modus können Sie nur Ihren Text personalisieren, Links hinzufügen oder Assets zu Ihrem Inhalt hinzufügen.

Sie können die gewünschten Änderungen am importierten Inhalt mit den [visuellen E-Mail-Editor-Tools](#add-structure-and-content) vornehmen.

### Vorlage auswählen {#choose-a-template}

Es gibt zwei Arten von Vorlagen zur Auswahl.

* Beispielvorlagen: Marketo Engage bietet vier vordefinierte E-Mail-Vorlagen.

* Gespeicherte Vorlagen: Hierbei handelt es sich um Vorlagen, die Sie im Menü Vorlagen neu erstellt haben, oder um eine E-Mail, die Sie erstellt und als Vorlage gespeichert haben.

>[!BEGINTABS]

>[!TAB Beispielvorlagen]

Wählen Sie eine der vordefinierten Vorlagen für einen Vorsprung im E-Mail-Vorlagenentwurf.

1. Der Tab Beispielvorlagen ist standardmäßig geöffnet.

1. Wählen Sie die Vorlage aus, die Sie verwenden möchten.

   ![](assets/authoring-sample-templates-1.png)

1. Klicken Sie auf **Diese Vorlage verwenden**.

   ![](assets/authoring-sample-templates-2.png)

1. Bearbeiten Sie den Inhalt nach Bedarf mit dem visuellen Inhaltsentwickler.

>[!TAB Gespeicherte Vorlagen]

1. Klicken Sie auf die Registerkarte **Gespeicherte Vorlagen** und wählen Sie die gewünschte Vorlage aus.

   ![](assets/authoring-saved-templates-1.png)

1. Klicken Sie auf **Diese Vorlage verwenden**.

   ![](assets/authoring-saved-templates-2.png)

1. Bearbeiten Sie den Inhalt nach Bedarf mit dem visuellen Inhaltsentwickler.

>[!ENDTABS]

## Hinzufügen von Struktur und Inhalt {#add-structure-and-content}

1. Um Inhalte zu erstellen oder zu ändern, ziehen Sie ein Element aus Strukturen auf die Arbeitsfläche. Bearbeiten Sie die Einstellungen im Bereich auf der rechten Seite.

   >[!TIP]
   >
   >Wählen Sie die n:n-Spaltenkomponente aus, um die Anzahl der Spalten Ihrer Wahl zu definieren (zwischen drei und zehn). Sie können auch die Breite jeder Spalte definieren, indem Sie die Pfeile unter die Spalte verschieben.

   ![](assets/authoring-add-structure-and-content-1.png)

   >[!NOTE]
   >
   >Die Spaltengröße darf nicht weniger als 10 % der Gesamtbreite der Strukturkomponente betragen. Es können nur leere Spalten entfernt werden.

1. Ziehen Sie aus dem Bereich Inhalt die gewünschten Elemente per Drag-and-Drop in eine oder mehrere Strukturkomponenten.

   ![](assets/authoring-add-structure-and-content-2.png)

1. Jede Komponente kann über die Registerkarten Einstellungen oder Stil angepasst werden. Ändern Sie Schriftart, Textstil, Rand und mehr.

### Assets hinzufügen {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY?
```

1. Um auf Ihre Bilder zuzugreifen, klicken Sie auf das Symbol Asset-Auswahl .

   SCREENSHOT

1. Ziehen Sie das gewünschte Bild in eine Strukturkomponente.

   SCREENSHOT

   >[!NOTE]
   >
   >Um ein vorhandenes Bild zu ersetzen, wählen Sie es aus und klicken Sie dann auf der Registerkarte Einstellungen auf der rechten Seite auf **Asset auswählen** .

Klicken Sie auf Bedingungsinhalt aktivieren , um dynamischen Inhalt hinzuzufügen und den Inhalt basierend auf Bedingungsregeln an die Zielprofile anzupassen.



Bei Bedarf können Sie Ihre E-Mail weiter personalisieren, indem Sie im erweiterten Menü auf In Code-Editor wechseln klicken. Dadurch können Sie den E-Mail-Quellcode bearbeiten, z. B. um Tracking- oder benutzerdefinierte HTML-Tags hinzuzufügen.

VORSICHT
Sie können nach dem Wechsel zum Code-Editor nicht zum visuellen Designer für diese E-Mail zurückkehren.

Sobald Ihr Inhalt fertig ist, klicken Sie auf die Schaltfläche Inhalt simulieren , um das Rendering zu überprüfen. Sie können zwischen der Desktop- oder der mobilen Ansicht wählen.

Wenn Sie fertig sind, klicken Sie auf Speichern .

### Ebenen, Einstellungen und Stile {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS
```

Öffnen Sie die Navigationsstruktur, um auf bestimmte Strukturen und deren Spalten/Komponenten zuzugreifen und so eine detailliertere Bearbeitung zu ermöglichen. Klicken Sie auf das Symbol Navigationsstruktur , um darauf zuzugreifen.

![](assets/authoring-layers-settings-styles-1.png)

Im folgenden Beispiel werden die Schritte zum Anpassen des Abstands und der vertikalen Ausrichtung innerhalb einer Strukturkomponente beschrieben, die aus Spalten besteht.

1. Wählen Sie die Spalte in der Strukturkomponente direkt auf der Arbeitsfläche aus oder verwenden Sie die links angezeigte _Navigationsstruktur_ .

1. Klicken Sie in der Spaltensymbolleiste auf das Tool _[!UICONTROL Spalte auswählen]_ und wählen Sie das Tool aus, das Sie bearbeiten möchten.

   Sie können sie auch im Strukturbaum auswählen. Die bearbeitbaren Parameter für diese Spalte werden auf den Registerkarten _[!UICONTROL Einstellungen]_ und _[!UICONTROL Stile]_ rechts angezeigt.

   ![](assets/authoring-layers-settings-styles-2.png)

1. Um die Spalteneigenschaften zu bearbeiten, klicken Sie auf die Registerkarte _[!UICONTROL Stile]_ rechts und ändern Sie sie entsprechend Ihren Anforderungen:

   * Ändern Sie für **[!UICONTROL Hintergrund]** die Hintergrundfarbe nach Bedarf.

     Deaktivieren Sie das Kontrollkästchen für einen transparenten Hintergrund. Aktivieren Sie die Einstellung **[!UICONTROL Hintergrundbild]** , um ein Bild als Hintergrund anstelle einer Vollbildfarbe zu verwenden.

   * Wählen Sie für **[!UICONTROL Ausrichtung]** das Symbol _Oben_, _Mitte_ oder _Unten_ aus.
   * Definieren Sie für **[!UICONTROL Abstand]** den Abstand für alle Seiten.

     Wählen Sie **[!UICONTROL Verschiedene Abstände für jede Seite]** aus, wenn Sie den Abstand anpassen möchten. Klicken Sie auf das Symbol _Sperren_ , um die Synchronisierung zu unterbrechen.

   * Erweitern Sie den Abschnitt **[!UICONTROL Erweitert]** , um Inline-Stile für die Spalte zu definieren.

   ![](assets/authoring-layers-settings-styles-3.png)

1. Wiederholen Sie diese Schritte nach Bedarf, um die Ausrichtung und den Abstand für die anderen Spalten in der Komponente anzupassen.

1. Speichern Sie Ihre Änderungen.

### Inhalt personalisieren {#personalize-content}

Token funktionieren im neuen Editor genauso wie im alten, aber das Symbol sieht anders aus. Im folgenden Beispiel wird das Hinzufügen eines Vorname-Tokens mit Fallback-Text beschrieben.

1. Wählen Sie die Textkomponente aus. Platzieren Sie den Cursor an die Stelle, an der das Token angezeigt werden soll, und klicken Sie auf das Symbol **Personalisierung hinzufügen** .

   ![](assets/authoring-personalize-content-1.png)

1. Klicken Sie auf den gewünschten [Token-Typ](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

   ![](assets/authoring-personalize-content-2.png)

1. Suchen Sie das gewünschte Token und klicken Sie auf das Symbol &quot;**...**&quot;. (Durch Klicken auf das Symbol &quot;+&quot;wird stattdessen ein Token ohne Fallback-Text hinzugefügt.)

   ![](assets/authoring-personalize-content-3.png)

   >[!NOTE]
   >
   >&quot;Fallback-Text&quot;ist der neue Editor-Begriff für den Standardwert. Beispiel: ``{{lead.First Name:default=Friend}}``. Dies wird empfohlen, falls im von Ihnen ausgewählten Feld kein Wert für die Person vorhanden ist.

1. Legen Sie Ihren Fallback-Text fest und klicken Sie auf **Hinzufügen**.

   ![](assets/authoring-personalize-content-4.png)

1. Klicken Sie auf **Speichern**.

### URL-Tracking bearbeiten {#edit-url-tracking}

Manchmal möchten Sie die Marketo-Tracking-URL nicht für einen Link in einer E-Mail aktivieren. Dies ist nützlich, wenn die Zielseite URL-Parameter nicht unterstützt und zu einem fehlerhaften Link führen kann.

1. Klicken Sie auf das Symbol Links , um alle URLs in Ihrer E-Mail anzuzeigen.

   ![](assets/authoring-edit-url-tracking-1.png)

1. Klicken Sie auf das Stiftsymbol, um das Tracking für alle gewünschten Links zu bearbeiten.

1. Klicken Sie auf die Dropdown-Liste **Trackingtyp** und wählen Sie aus.

   ![](assets/authoring-edit-url-tracking-2.png)

   ```
   LABEL?
   
   TAGS?
   ```

   <table><tbody>
     <tr>
       <td><b>Tracking ohne mkt_tok</b></td>
       <td>Definition</td>
     </tr>
     <tr>
       <td><b>Tracking mit mkt_tok</b></td>
       <td>Definition</td>
     </tr>
     <tr>
       <td><b>Nicht verfolgen</b></td>
       <td>Definition</td>
     </tr>
   </tbody>
   </table>

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

## Warnhinweise überprüfen {#check-alerts}

Bei der Inhaltserstellung werden Warnhinweise oben rechts im Bildschirm angezeigt, wenn wichtige Einstellungen fehlen.

Es gibt zwei Arten von Warnhinweisen:

**Warnungen**

Warnungen beziehen sich auf Empfehlungen und Best Practices, z. B.:

* **Der Abmelde-Link ist nicht im E-Mail-Textkörper enthalten**: Obwohl Abmelde-Links eine Anforderung darstellen, empfiehlt sich, sie dem Hauptteil Ihrer E-Mail hinzuzufügen.

>[!NOTE]
>
>Das Hinzufügen einer Abmeldeoption ist für [operative E-Mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (Nicht-Marketing) nicht erforderlich.

* **Textversion von HTML ist leer**: Sie müssen eine Textversion Ihres E-Mail-Textkörpers definieren, für die kein HTML-Inhalt angezeigt werden kann.

* **Leerer Link ist im E-Mail-Textkörper vorhanden**: Überprüfen Sie, ob alle Links in Ihrer E-Mail korrekt sind.

* **Die E-Mail-Größe hat die Grenze von 100 KB überschritten**: Stellen Sie für einen optimalen Versand sicher, dass die Größe Ihrer E-Mail 100 KB nicht überschreitet.

**Fehler**

Fehler verhindern, dass Sie die E-Mail senden oder testen, bis sie behoben sind:

* **Betreffzeile fehlt**: Eine E-Mail-Betreffzeile ist erforderlich.

* **E-Mail-Version der Nachricht ist leer**: Dieser Fehler tritt auf, wenn der E-Mail-Inhalt nicht konfiguriert wurde.

## E-Mail testen {#test-your-email}

Wenn Ihr Nachrichteninhalt definiert ist, können Sie mithilfe von Testprofilen die Vorschau anzeigen, Testsendungen durchführen und steuern, wie die Nachricht in beliebten Desktop-, Mobile- und Web-basierten Clients dargestellt wird. Wenn Sie personalisierten Inhalt eingefügt haben, können Sie anhand von Testprofildaten überprüfen, wie dieser in der Nachricht angezeigt wird.

Um eine Vorschau Ihres E-Mail-Inhalts anzuzeigen, klicken Sie auf **Inhalt simulieren** und fügen Sie dann ein Testprofil hinzu, um Ihre Nachricht mithilfe der Testprofildaten zu überprüfen.

![](assets/test-your-email-1.png)

## E-Mail referenzieren {#reference-an-email}

Nachdem Sie eine E-Mail im neuen Editor erstellt haben, können Sie sie in Smart-Kampagnen und/oder Smart-Listen wie bei jeder anderen E-Mail referenzieren.

* Verweisen Sie in einer Smart-Liste darauf, indem Sie [die üblichen Schritte befolgen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Verweisen Sie in einer Smart-Kampagne darauf, indem Sie [die üblichen Schritte befolgen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Nur gespeicherte E-Mails können referenziert werden. Im neuen E-Mail-Editor gibt es keinen Status &quot;Genehmigt&quot;.

>[!MORELIKETHIS]
>
>[E-Mail-Vorlagen](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-templates.md){target="_blank"}: Erfahren Sie, wie Sie eine E-Mail-Vorlage im neuen Editor erstellen, entwerfen und darauf zugreifen.
