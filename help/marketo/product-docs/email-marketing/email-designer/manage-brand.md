---
solution: Marketo Engage
product: Marketo
title: Verwalten von Marken
description: Erfahren Sie, wie Sie Markenrichtlinien erstellen und verwalten
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '1410'
ht-degree: 84%

---

# Erstellen und Verwalten von Marken {#brands}

Markenrichtlinien sind ein detaillierter Satz an Regeln und Standards, die die visuelle und sprachliche Identität einer Marke festlegen. Sie dienen als Referenz, um eine konsistente Markendarstellung über alle Marketing- und Kommunikationsplattformen hinweg aufrechtzuerhalten.

Manuelle Eingabe und Organisation Ihrer Markendetails oder Hochladen von Dokumenten zu Markenrichtlinien für die automatische Extraktion von Informationen.

>[!AVAILABILITY]
>
>Sie müssen der [Benutzervereinbarung“ zustimmen](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} bevor Sie den KI-Assistenten in Adobe Marketo Engage verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

## Zugriff auf Marken {#generative-access}

Um auf das Menü **[!UICONTROL Marken]** in [!DNL Adobe Marketo Engage] zugreifen zu können, müssen Benutzenden die Berechtigungen **[!UICONTROL Markenkit verwalten]** oder **[!UICONTROL KI-Assistenten aktivieren]**.

+++  Informationen zur Zuweisung von Markenberechtigungen

Gehen Sie wie folgt vor, um Marken Berechtigungen zuzuweisen:

1. Gehen Sie im Produkt **Berechtigungen** zur Registerkarte **Rollen** und wählen Sie die gewünschte **Rolle** aus.

1. Klicken Sie auf **Bearbeiten**, um die Berechtigungen zu ändern.

1. Fügen Sie die Ressource **KI-Assistent** hinzu und wählen Sie dann aus dem Dropdown-Menü die Option **Marken-Kit verwalten** oder **[!UICONTROL KI-Assistenten aktivieren]** aus.

   Beachten Sie, dass die Berechtigung **[!UICONTROL KI-Assistenten aktivieren]** nur schreibgeschützten Zugriff auf das Menü **[!UICONTROL Marken]** bietet.

   SCREENSHOT

1. Klicken Sie auf **Speichern**, um die Änderungen anzuwenden.

   Die Berechtigungen aller Benutzenden, die dieser Rolle bereits zugewiesen sind, werden automatisch aktualisiert.

1. Um diese Rolle neuen Benutzenden zuzuweisen, navigieren Sie im Dashboard **Rollen** zur Registerkarte **Benutzer** und klicken Sie auf **Benutzer hinzufügen**.

1. Geben Sie den Namen und die E-Mail-Adresse der Benutzerin oder des Benutzers ein oder wählen Sie aus der Liste aus und klicken Sie dann auf **Speichern**.

1. Wenn die Benutzerin bzw. der Benutzer vorher noch nicht erstellt wurde, lesen Sie [diese Dokumentation](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/abac/permissions-ui/users).

+++

## Erstellen und Verwalten Ihrer Marke {#create-brand-kit}

Zum Erstellen und Verwalten Ihrer Markenrichtlinie können Sie die Details entweder selbst eingeben oder Ihr Dokument mit den Markenrichtlinien hochladen, damit die Informationen automatisch extrahiert werden:

1. Klicken Sie im Menü **[!UICONTROL Marken]** auf **[!UICONTROL Marke erstellen]**.

   SCREENSHOT

1. Geben Sie einen **[!UICONTROL Namen]** für Ihre Marke ein.

1. Ziehen Sie Ihre Datei per Drag-and-Drop oder wählen Sie sie aus, um Ihre Markenrichtlinien hochzuladen und relevante Markeninformationen automatisch zu extrahieren. Klicken Sie auf **[!UICONTROL Marke erstellen]**.

   Der Prozess zur Informationsextraktion beginnt jetzt. Beachten Sie, dass der Prozess mehrere Minuten in Anspruch nehmen kann.

   SCREENSHOT

1. Ihre Standards für Content und visuelle Erstellung werden jetzt automatisch ausgefüllt. Gehen Sie die verschiedenen Registerkarten durch, um die Informationen nach Bedarf anzupassen. [Weitere Informationen](#personalize)

1. Im erweiterten Menü jedes Abschnitts bzw. jeder Kategorie können Sie Verweise hinzufügen, um relevante Markeninformationen automatisch zu extrahieren.

   Um vorhandene Inhalte zu entfernen, verwenden Sie die Optionen **[!UICONTROL Abschnitt löschen]** oder **[!UICONTROL Kategorie löschen]**.

   SCREENSHOT

1. Klicken Sie nach der Konfiguration auf **[!UICONTROL Speichern]** und dann auf **[!UICONTROL Veröffentlichen]**, um Ihre Markenrichtlinie im KI-Assistenten verfügbar zu machen.

1. Um Änderungen an Ihrer veröffentlichten Marke vorzunehmen, klicken Sie auf **[!UICONTROL Marke bearbeiten]**.

   >[!NOTE]
   >
   >Dadurch wird eine temporäre Kopie im Bearbeitungsmodus erstellt, die die Live-Version nach der Veröffentlichung ersetzt.

   SCREENSHOT

1. Öffnen Sie im Dashboard **[!UICONTROL Marken]** das erweiterte Menü, indem Sie auf die drei Punkte klicken, um Folgendes zu tun:

   * Marke anzeigen
   * Bearbeiten
   * Duplizieren
   * Veröffentlichen
   * Veröffentlichung aufheben
   * Löschen

   SCREENSHOT

Ihre Markenrichtlinien sind jetzt über die Dropdown-Liste **[!UICONTROL Marke]** im Menü KI-Assistent verfügbar, sodass Inhalte und Assets generiert werden können, die mit Ihren Spezifikationen übereinstimmen.

SCREENSHOT

### Festlegen einer Standardmarke {#default-brand}

Sie können eine Standardmarke festlegen, die beim Generieren von Inhalten und Berechnen der Ausrichtungswerte während der Kampagnenerstellung automatisch angewendet wird.

Um eine Standardmarke festzulegen, gehen Sie zum Dashboard **[!UICONTROL Marken]**. Öffnen Sie das erweiterte Menü, indem Sie auf das Symbol mit den drei Punkten klicken und **[!UICONTROL Als Standardmarke markieren]** auswählen.

SCREENSHOT

## Personalisieren Ihrer Marke {#personalize}

### Informationen zur Marke {#about-brand}

Verwenden Sie die Registerkarte **[!UICONTROL Informationen zur Marke]**, um die Kernidentität Ihrer Marke festzulegen und Zweck, Persönlichkeit, Tagline und andere definierende Attribute darzulegen.

1. Füllen Sie zunächst die grundlegenden Informationen für Ihre Marke in der Kategorie **[!UICONTROL Schlüsseldetails]** aus:

   * **[!UICONTROL Marken-Kit-Name]**: Geben Sie den Namen Ihres Marken-Kits ein.

   * **[!UICONTROL Verwendung]**: Geben Sie Szenarien oder Kontexte an, in denen dieses Marken-Kit verwendet werden soll.

   * **[!UICONTROL Markenname]**: Geben Sie den offiziellen Namen der Marke ein.

   * **[!UICONTROL Markenbeschreibung]**: Geben Sie einen Überblick darüber, wofür diese Marke steht.

   * **[!UICONTROL Standard-Tagline]**: Fügen Sie die primäre Tagline für die Marke hinzu.

   SCREENSHOT

1. Spezifizieren Sie in der Kategorie **[!UICONTROL Leitprinzipien]** die Kernausrichtung und -philosophie Ihrer Marke:

   * **[!UICONTROL Mission]**: Beschreiben Sie den Zweck Ihrer Marke.

   * **[!UICONTROL Vision]**: Beschreiben Sie das langfristige Ziel oder den gewünschten zukünftigen Status.

   * **[!UICONTROL Marktpositionierung]**: Erklären Sie, wie Ihre Marke auf dem Markt positioniert ist.

   SCREENSHOT

1. Klicken Sie in der Kategorie **[!UICONTROL Core]** Markenwerte“ auf „Symbol hinzufügen“, um die Kernwerte der Marke hinzuzufügen und die Details auszufüllen:

   * **[!UICONTROL Wert]**: Benennen Sie einen Kernwert der Marke.

   * **[!UICONTROL Beschreibung]**: Erklären Sie, was dieser Wert für Ihre Marke bedeutet.

   * **[!UICONTROL Verhaltensweisen]**: Beschreiben Sie Aktionen oder Haltungen, die diesen Wert in der Praxis widerspiegeln.

   * **[!UICONTROL Manifestationen]**: Geben Sie Beispiele dafür, wie dieser Wert beim realen Branding ausgedrückt wird.

   SCREENSHOT

1. Klicken Sie bei Bedarf auf das Symbol „Bearbeiten“, um einen Ihrer Markenwerte zu aktualisieren oder zu löschen.

   SCREENSHOT

Nun können Sie Ihre Marke weiter personalisieren oder [veröffentlichen](#create-brand-kit).

### Schreibstil {#writing-style}

Im Abschnitt **[!UICONTROL Schreibstil]** werden die Standards zum Verfassen von Inhalten beschrieben. Es wird festgelegt, wie Sprache, Formatierung und Struktur verwendet werden sollten, um Klarheit, Kohärenz und Konsistenz in allen Materialien sicherzustellen.

+++ Verfügbare Kategorien und Beispiele

<table>
  <thead>
    <tr>
      <th>Kategorie</th>
      <th>Unterkategorie</th>
      <th>Beispiel für Richtlinien</th>
      <th>Beispiel für Ausschlüsse</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Inhaltserstellungsstandards</td>
      <td>Markenbotschaftsstandards</td>
      <td>Heben Sie Innovation und die Bedeutung der Kundinnen und Kunden hervor.</td>
      <td>Versprechen Sie nicht zu viel in Bezug auf Produktfunktionen.</td>
    </tr>
    <tr>
      <td>Tagline-Nutzung</td>
      <td>Platzieren Sie die Tagline unter dem Logo auf allen Digital-Marketing-Assets.</td>
      <td>Verändern oder übersetzen Sie die Tagline nicht.</td>
    </tr>
    <tr>
      <td>Kernbotschaften</td>
      <td>Betonen Sie den Hauptvorteil betonen, z. B. verbesserte Produktivität.</td>
      <td>Verwenden Sie keine Werteversprechen ohne Bezug.</td>
    </tr>
    <tr>
      <td>Benennungsstandards</td>
      <td>Verwenden Sie einfache, beschreibende Namen verwenden, z. B. „ProScheduler“.</td>
      <td>Verwenden Sie keine komplexen Begriffe und Sonderzeichen.</td>
    </tr>
    <tr>
      <td rowspan="5">Stil für Markenkommunikation</td>
      <td>Eigenschaften der Markenpersönlichkeit</td>
      <td>Freundlich und zugänglich.</td>
      <td>Seien Sie nicht pessimistisch.</td>
    </tr>
    <tr>
      <td>Schreibtechnik</td>
      <td>Formulieren Sie kurze und prägnante Sätze.</td>
      <td>Verwenden Sie nicht übermäßig viel Jargon.</td>
    </tr>
    <tr>
      <td>Situationsbezogener Ton</td>
      <td>Behalten Sie einen professionellen Tonfall in der Kommunikation in Krisensituationen bei.</td>
      <td>Seien Sie bei Support-Interaktionen nicht herablassend.</td>
    </tr>
    <tr>
      <td>Richtlinien zur Wortwahl</td>
      <td>Verwenden Sie Wörter wie „innovativ“ und „intelligent“.</td>
      <td>Vermeiden Sie Wörter wie „billig“ oder „Hack“.</td>
    </tr>
    <tr>
      <td>Sprachstandards</td>
      <td>Befolgen Sie die Konventionen von amerikanischem Englisch.</td>
      <td>Vermischen Sie britische und amerikanische Rechtschreibung nicht.</td>
    </tr>
    <tr>
      <td rowspan="3">Standards zur Einhaltung gesetzlicher Vorschriften</td>
      <td>Markenzeichenstandards</td>
      <td>Verwenden Sie die Symbole ™ oder ® immer.</td>
      <td>Lassen Sie rechtliche Symbole nicht weg, wenn sie erforderlich sind.</td>
    </tr>
    <tr>
      <td>Copyright-Standards</td>
      <td>Geben Sie Urheberrechtsvermerke auf Marketing-Materialen an.</td>
      <td>Verwenden Sie Inhalte von Dritten nicht ohne Berechtigung.</td>
    </tr>
    <tr>
      <td>Haftungsausschlussstandards</td>
      <td>Zeigen Sie Haftungsausschlüsse deutlich lesbar auf digitalen Assets an.</td>
      <td>Verstecken Sie Haftungsausschlüsse nicht in nicht sichtbaren Bereichen.</td>
    </tr>
</table>

+++

</br>

So personalisieren Sie Ihren **[!UICONTROL Schreibstil]**:

1. Klicken Sie auf der **[!UICONTROL Schreibstil]** auf das Symbol **+** , um eine Richtlinie, einen Ausnahmefehler oder einen Ausschluss hinzuzufügen.

1. Geben Sie die Richtlinie, die Ausnahme oder den Ausschluss ein. Sie können auch **[!UICONTROL Beispiele]** hinzufügen, um die Anwendung besser zu veranschaulichen.

   SCREENSHOT

1. Geben Sie den Verwendungskontext für die Richtlinie, die Ausnahme oder den Ausschluss an:

   * **[!UICONTROL Kanaltyp]**: Wählen Sie aus, wo die Richtlinie, die Ausnahme oder der Ausschluss gelten soll. Beispielsweise soll möglicherweise ein bestimmter Schreibstil nur in E-Mail-, Mobile-, Print- oder anderen Kommunikationskanälen verwendet werden.

   * **[!UICONTROL Elementtyp]**: Geben Sie an, für welches Inhaltselement die Regel gilt. Das können Elemente wie Überschriften, Schaltflächen, Links oder andere Komponenten in Ihrem Inhalt sein.

   SCREENSHOT

1. Nachdem Sie die Richtlinie, die Ausnahme oder den Ausschluss eingerichtet haben, klicken Sie auf **[!UICONTROL Hinzufügen]**.

1. Wählen Sie bei Bedarf eine Richtlinie oder einen Ausschluss zum Aktualisieren oder Löschen aus.

1. Klicken Sie auf „Bearbeiten“, um Ihr Beispiel zu bearbeiten, oder auf das Symbol „Löschen“, um es zu löschen.

   SCREENSHOT

Nun können Sie Ihre Marke weiter personalisieren oder [veröffentlichen](#create-brand-kit).

### Visueller Inhalt {#visual-content}

Im Abschnitt **[!UICONTROL Visueller Inhalt]** werden die Standards für Bilder und Design definiert. Darin werden die Spezifikationen beschrieben, die für einen einheitlichen und konsistenten Look der Marke erforderlich sind.

+++ Verfügbare Kategorien und Beispiele

<table>
  <thead>
    <tr>
      <th>Kategorie</th>
      <th>Beispiel für Richtlinien</th>
      <th>Beispiel für Ausschlüsse</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fotografiestandards</td>
      <td>Verwenden Sie natürliches Licht für Außenaufnahmen.</td>
      <td>Vermeiden Sie stark bearbeitete oder verpixelte Bilder.</td>
    </tr>
    <tr>
      <td>Illustrationsstandards</td>
      <td>Verwenden Sie klare und minimalistische Stile.</td>
      <td>Vermeiden Sie zu komplexe Veranschaulichungen.</td>
    </tr>
    <tr>
      <td>Symbolstandards</td>
      <td>Verwenden Sie ein konsistentes 24-px-Rastersystem.</td>
      <td>Vermischen Sie keine Symbolabmessungen, verwenden Sie keine inkonsistenten Strichstärken und weichen Sie nicht von Rasterregeln ab.</td>
    </tr>
    <tr>
      <td>Nutzungsrichtlinien</td>
      <td>Wählen Sie Lifestyle-Bilder, die reale Kundinnen und Kunden widerspiegeln, die das Produkt in professionellen Umgebungen verwenden.</td>
      <td>Verwendne Sie keine Bilder, die dem Ton der Marke widersprechen oder anscheinend aus dem Zusammenhang gerissen sind.</td>
    </tr>
</table>

+++

</br>

So personalisieren Sie Ihren **[!UICONTROL visuellen Inhalt]**:

1. Klicken Sie auf der Registerkarte **[!UICONTROL Visueller]**) auf das Symbol mit den drei Punkten, um eine Richtlinie, einen Ausschluss oder ein Beispiel hinzuzufügen.

1. Geben Sie die Richtlinie, den Ausschluss oder ein Beispiel ein.

   SCREENSHOT

1. Geben Sie den Verwendungskontext für die Richtlinie oder den Ausschluss an:

   * **[!UICONTROL Kanaltyp]**: Wählen Sie aus, wo die Richtlinie, die Ausnahme oder der Ausschluss gelten soll. Beispielsweise soll möglicherweise ein bestimmter Schreibstil nur in E-Mail-, Mobile-, Print- oder anderen Kommunikationskanälen verwendet werden.

   * **[!UICONTROL Elementtyp]**: Geben Sie an, für welches Inhaltselement die Regel gilt. Das können Elemente wie Überschriften, Schaltflächen, Links oder andere Komponenten in Ihrem Inhalt sein.

   SCREENSHOT

1. Nachdem Sie die Richtlinie, die Ausnahme oder den Ausschluss eingerichtet haben, klicken Sie auf **[!UICONTROL Hinzufügen]**.

1. Um ein Bild zum Veranschaulichen der korrekten Verwendung hinzuzufügen, wählen Sie **[!UICONTROL Beispiel]** und klicken Sie auf **[!UICONTROL Bild auswählen]**. Sie können auch ein Bild zur Veranschaulichung der inkorrekten Verwendung als Ausschlussbeispiel hinzufügen.

   SCREENSHOT

1. Wählen Sie bei Bedarf eine Richtlinie oder einen Ausschluss zum Aktualisieren oder Löschen aus.

1. Wählen Sie eine Richtlinie oder einen Ausschluss aus, um diese bzw. diesen zu aktualisieren. Klicken Sie auf das Symbol „Löschen“, um es zu löschen.

   SCREENSHOT

Nun können Sie Ihre Marke weiter personalisieren oder [veröffentlichen](#create-brand-kit).
