---
solution: Marketo Engage
product: marketo
title: Vorlagenimport
description: Erfahren Sie, wie Sie Ihre vorhandenen E-Mail-Vorlagen aus dem klassischen Editor in die neue E-Mail-Designer importieren.
level: Beginner, Intermediate
feature: Email Designer
badge: Beta
hide: true
hidefromtoc: true
source-git-commit: 316d5b59c7ea573f9246613ab3df2de86bdf4706
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 1%

---

# Vorlagenimport {#template-import}

Importieren Sie Ihre vorhandenen E-Mail-Vorlagen nahtlos aus dem klassischen Editor in die neue E-Mail-Designer, behalten Sie Ihre Designs bei und beschleunigen Sie die Vorlagenerstellung mit vertrauten, wiederverwendbaren Strukturen. Lesen Sie [Best Practices](#best-practices) und erfahren Sie mehr über [Einschränkungen und Abhilfemaßnahmen](#limitations-and-remedies).

1. Gehen Sie zum **Design Studio**.

   SCREENSHOT

1. Klicken Sie auf **E-Mail** Vorlagen) und wählen Sie **E-Mail-Vorlagen (Neu)**.

   SCREENSHOT

1. Klicken Sie **Vorlage erstellen**.

   SCREENSHOT

1. Geben Sie _Name_ und (optional) _Beschreibung_ ein.

   SCREENSHOT

1. Klicken Sie auf die **Marketo** Vorlagen und wählen Sie die vorhandenen Vorlagen aus, die im klassischen E-Mail-Editor erstellt wurden.

   SCREENSHOT

   >[!NOTE]
   >
   >Nur genehmigte Vorlagen und Vorlagen, die für den aktuellen Arbeitsbereich freigegeben wurden, können importiert werden.

1. Wählen Sie die gewünschte Vorlage aus.

   SCREENSHOT

1. Klicken Sie auf Diese Vorlage verwenden .

   SCREENSHOT

1. Die importierte Vorlage wird in der E-Mail-Designer geöffnet.

1. Überprüfen Sie die Komponenten auf korrekte Konvertierung und nehmen Sie mithilfe der Designer die gewünschten Anpassungen vor. Wenn Sie mit der Vorlage zufrieden sind, genehmigen Sie sie für die Verwendung in E-Mails.

## Erstellen von Fragmenten {#create-fragments}

Es empfiehlt sich, Fragmente wiederholbarer Abschnitte zur späteren Verwendung zu erstellen.

1. Klicken Sie oben auf die Schaltfläche **…** und wählen Sie **Als Fragment speichern**.

   SCREENSHOT

1. Wählen Sie eine Komponente oder Struktur aus und klicken Sie auf **Erstellen**.

   SCREENSHOT

1. Geben Sie einen Namen (und optional eine Beschreibung) ein und klicken Sie auf **Speichern**.

   SCREENSHOT

## Best Practices {#best-practices}

* Da der Freestyle HTML erheblich variieren kann, interpretiert der Importer möglicherweise nicht immer alle Komponenten perfekt. Überprüfen Sie Ihre importierten Vorlagen, um sicherzustellen, dass alle Abschnitte bearbeitbar und korrekt zugeordnet sind. Wenn ein Bauteil nicht ausgewählt werden kann, müssen Sie diesen Abschnitt einfach neu erstellen, um ein optimales Ergebnis zu erzielen.

* Nach dem Import können Sie wiederverwendbare Abschnitte als Fragmente speichern und für die Verwendung durch E-Mail-Autoren genehmigen. Wenden Sie Markendesigns an, um Konsistenz und Konformität zu gewährleisten.

* Sie können die Velocity-Skripterstellung fortsetzen und ältere Snippets mit einer Kombination aus Fragmenten und bedingten Inhalten erneut implementieren, um die Flexibilität und Kontrolle zu verbessern.

## Einschränkungen und Abhilfemaßnahmen {#limitations-and-remedies}

<table><thead>
  <tr>
    <th>Einschränkung</th>
    <th>Grund</th>
    <th>Rechtsmittel</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Die im klassischen E-Mail-Editor definierten Variablen sind nicht auf E-Mail-Ebene verfügbar.</td>
    <td>Die Variablen wurden ursprünglich entwickelt, um die E-Mail-Bearbeitung zu vereinfachen, als der Editor noch keine WYSIWYG-Funktionen bot. In der E-Mail-Designer können Benutzende durch die verfügbaren Steuerelemente eine ähnliche Flexibilität erzielen. Das Import-Tool verwaltet die Struktur und Komponenten der vorhandenen Vorlage und hilft Ihnen, sie effizient in der E-Mail-Designer neu zu erstellen.</td>
    <td>Benutzer sollten dies in der Designer erreichen können. <p>
    Bei -Modulen können Sie verschiedene Segmente als Fragmente speichern. Genehmigte Fragmente sind zur Verwendung auf E-Mail-Ebene verfügbar.</td>
  </tr>
  <tr>
    <td>Wenn die Quell-HTML verschachtelte Blöcke enthält, sind die tieferen Ebenen in der Designer nicht adressierbar.</td>
    <td>Verschachtelte Kommentare werden von E-Mail-Designer nicht unterstützt.</td>
    <td>Obwohl Designer die Bearbeitung verschachtelter Strukturen nicht zulässt, sollte es genau gerendert werden. Achten Sie darauf, zuerst die Vorlage zu testen.<p>
    Erstellen Sie die Struktur mithilfe des Rasters neu.</td>
  </tr>
  <tr>
    <td>Manchmal werden Schaltflächen als einfache Container mit Text darin importiert.</td>
    <td>Einige Implementierungsstile, die HTML verwenden, können beim Import falsch ausgelegt werden.</td>
    <td>Erstellen Sie die Schaltfläche in der Designer neu.</td>
  </tr>
  <tr>
    <td>Schaltflächen können manchmal übergroß sein.</td>
    <td>Konflikt zwischen CSS der Marketo-E-Mail und anderen Elementen der unteren Ebene (<code>&lt;span&gt;</code>)</td>
    <td>Passen Sie die Ränder und Abstände der Schaltfläche in der Designer an.</td>
  </tr>
  <tr>
    <td>Aufzählungspunkte werden nativ nicht unterstützt.</td>
    <td>Die E-Mail-Designer bietet derzeit keine Aufzählungspunkte.</td>
    <td>Erwägen Sie die erneute Implementierung von Aufzählungszeichen mithilfe alternativer Techniken.</td>
  </tr>
  <tr>
    <td>Die vertikale Ausrichtung ist verzerrt, wenn der Inhalt des Containers nicht den Wert des Attributs „valign“ berücksichtigt.</td>
    <td><code>valign</code> funktioniert nicht in Containern, die in der Vorlage definiert sind.</td>
    <td>Passen Sie Ränder und Abstände der Schaltfläche in der E-Mail-Designer an.</td>
  </tr>
  <tr>
    <td>Personalization-Token (Meine Token) auf Programmebene auf Vorlagenebene können zu Validierungsfehlern führen.</td>
    <td>E-Mail-Vorlagen unterstützen keine Token auf Programmebene.</td>
    <td>Ersetzen Sie sie durch andere Token-Typen in Vorlagen und ersetzen Sie sie durch „Meine Token“ in den einzelnen E-Mails.</td>
  </tr>
  <tr>
    <td>Unterteilungskomponenten sind möglicherweise nicht auswählbar.</td>
    <td>Trennzeichenkomponenten werden in dieser Version nicht behandelt.</td>
    <td>k. A.</td>
  </tr>
  <tr>
    <td>Wenn der HTML noch irgendwelche Strukturen hat, die nicht richtig geformt sind, dann werden diese wahrscheinlich übernommen.</td>
    <td>Probleme mit dem Original-HTML.</td>
    <td>Die Probleme müssen vor dem Import behoben werden.</td>
  </tr>
  <tr>
    <td>Für den importierten Inhalt ist die Verwendung der Inhaltsvorschau kein zuverlässiger Indikator.</td>
    <td>Die Vorschaufunktion von Designer unterstützt keine benutzerdefinierte HTML.</td>
    <td>Es wird empfohlen, Ihre E-Mail mit der Option <b>Testversand durchführen</b> im Bildschirm <i>Inhalt simulieren</i> zu testen.</td>
  </tr>
  <tr>
    <td>Die Snippets in der alten Vorlage funktionieren in der E-Mail-Designer nicht.</td>
    <td>E-Mail-Designer unterstützt keine Snippets.</td>
    <td>Implementieren Sie Ihre Ausschnitte als Fragmente zusammen mit bedingten Inhalten erneut.</td>
  </tr>
</tbody></table>
