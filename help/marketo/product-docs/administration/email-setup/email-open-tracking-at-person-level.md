---
description: Beschreibung
title: Öffnungs-Tracking von E-Mails auf Personenebene
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 387abcce00de365f2b4abda9565b0eada2598cfd
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 3%
---
# Öffnungs-Tracking von E-Mails auf Personenebene {#email-open-tracking-at-person-level}

Steuern Sie, ob Adobe Marketo Engage E-Mail-Öffnungen und -Klicks für jede Person verfolgt. Mit E-Mail-Tracking-Überschreibungen auf Personenebene können Sie einen Standard auf Instanzebene anwenden und diesen Standard dann für einzelne Personen ändern. Öffnungs- und Klick-Tracking werden unabhängig gesteuert.

Verwenden Sie diese Funktion, wenn Ihre Datenschutzanforderungen oder Unternehmensrichtlinien eine Zustimmung erfordern, bevor E-Mail-Interaktionen verfolgt werden.

>[!IMPORTANT]
> 
>Diese Funktion bietet Steuerelemente, die Sie bei der Erfüllung Ihrer Compliance-Verpflichtungen unterstützen können. Es wird nicht festgelegt, welche Gesetze gelten oder welche Personen ihr Einverständnis geben müssen. Arbeiten Sie mit Ihren Rechts- und Datenschutzteams zusammen, um zu entscheiden, wie Sie das Tracking konfigurieren und Einverständnis erfassen und aufbewahren.

## Funktionsweise von Tracking-Entscheidungen

Drei Einstellungen funktionieren zusammen:

| Einstellung | Ebene | Funktion |
|---|---|---|
| **Überschreibungen des E-Mail-Trackings auf Benutzerebene** | Instanz | Schaltet die Funktion ein oder aus. Wenn diese Option deaktiviert ist, ignoriert Marketo Engage die standardmäßigen Instanzfelder und Personenüberschreibungsfelder und verwendet ein normales Tracking-Verhalten. |
| **E-Mail-Tracking standardmäßig deaktiviert** | Instanz | Legt die Standardeinstellung für Öffnungs- und Klick-Tracking fest. Wenn diese Option deaktiviert ist, ist das Tracking standardmäßig aktiviert. Wenn diese Option aktiviert ist, ist das Tracking standardmäßig deaktiviert. |
| **Offene Tracking-Standard überschreiben** und **Klick-Tracking-Standard überschreiben** | Person | Boolesche Personenfelder. Der Wert `true` wendet das Gegenteil des Instanzstandards für diesen Tracking-Typ an. Der Wert `false` oder ein leerer Wert folgt dem Standardwert der Instanz. |

Die Überschreibungsfelder bedeuten nicht allein „Opt-in“ oder „Opt-out“. **`true`bedeutet immer „das Gegenteil der Standardinstanz“**

### Tabelle der Tracking-Entscheidungen

Marketo Engage wendet diese Entscheidung separat auf E-Mail-Öffnungen und E-Mail-Klicks an.

| Funktion | Instance default | Personenüberschreibungen sind `false` oder leer | Personenüberschreibungen sind `true` |
|---|---|---|---|
| Ein | Standardmäßig wird Tracking für ausgeführt | Getrackt | Nicht aktiviert |
| Ein | Standardmäßig nachverfolgen | Nicht aktiviert | Getrackt |
| Aus | Nicht zutreffend | Normales Tracking; Überschreiben und Standard werden ignoriert | Normales Tracking; Überschreiben und Standard werden ignoriert |

### Beispiel

Angenommen, die Funktion ist aktiviert und das Tracking der Instanz erfolgt standardmäßig. Für eine Person ist **Standard für Öffnungs-Tracking überschreiben** auf `true` festgelegt, während **Standard für Klick-Tracking überschreiben** leer ist. Marketo Engage verfolgt die E-Mail-Öffnungen dieser Person nicht, verfolgt aber weiterhin deren E-Mail-Klicks.

## Tracking-Modell auswählen

Wählen Sie das Modell aus, das Ihren Einverständnis- und Datenschutzanforderungen entspricht, bevor Sie die Funktion aktivieren oder Personenfelder ausfüllen.

| Modell | Instance default | Setzen Sie die Überschreibung auf `true`, wenn | Typische Verwendung |
|---|---|---|---|
| Opt-out | Standardmäßig wird Tracking für ausgeführt | Person widerspricht dem Tracking | Verfolgen Sie die meisten Personen, aber hören Sie auf, Personen zu verfolgen, die Einwände erheben. |
| Opt-in (Einverständnis) | Standardmäßig nachverfolgen | Eine Person erteilt ihre Zustimmung zum Tracking | Einverständnis vor dem Tracking verlangen, auch für Empfänger, die unter die geltenden CNIL- oder Garantieleitlinien fallen. |

>[!CAUTION]
> 
>Wählen Sie Ihr Modell aus, bevor Sie die Felder zum Überschreiben ausfüllen, und vermeiden Sie es, den Standardwert der Instanz nachträglich zu ändern. Da `true` „das Gegenteil des Standardwerts“ bedeutet, wird durch die Änderung des Standardwerts der Effekt jeder vorhandenen Überschreibung rückgängig gemacht. Wenn Sie beispielsweise von der standardmäßigen Tracking-Funktion auf die standardmäßige Tracking-Funktion wechseln, können Personen verfolgt werden, die dieser Tracking-Funktion zuvor widersprochen haben. Wenn Sie die Standardeinstellung ändern müssen, aktualisieren Sie die Überschreibungswerte für alle betroffenen Personen, bevor die Änderung wirksam wird.

## Funktion einschalten

Überschreibungen des E-Mail-Trackings auf Personenebene sind standardmäßig deaktiviert. Um sie zu aktivieren, wenden Sie sich an den Kunden-Support von Adobe und geben Sie Folgendes an:

1. Dass Sie Überschreibungen des E **Mail-Trackings auf Benutzerebene aktivieren**.
2. Gibt an, ob die Standardinstanz **standardmäßig aktiviert“ oder**&#x200B;**standardmäßig deaktiviert** lauten soll.

>[!TIP]
> 
>Füllen Sie die Felder zum Überschreiben für bestehende Personen aus, bevor Sie Adobe bitten, die Funktion zu aktivieren. Dadurch wird sichergestellt, dass das beabsichtigte Tracking-Verhalten ab der ersten E-Mail gilt, die nach der Aktivierung vorbereitet wurde.

## Festlegen von Überschreibungswerten für Personen

Die Überschreibungsfelder sind boolesche Personenfelder. Legen Sie sie mithilfe der Methode fest, die zu Ihrem Workflow passt:

| Methode | Hinweise |
|---|---|
| Schritt „Datenwertfluss ändern“ | Verwenden Sie eine intelligente Kampagne, um ein Feld festzulegen, wenn eine Person Ihre Kriterien erfüllt, z. B. ein Einverständnis-Kontrollkästchen in einem Formular übermitteln. |
| Formulare | Ordnen Sie ein Kontrollkästchen oder ein ausgeblendetes Feld in einem Marketo Engage-Formular dem Personenfeld zu. |
| Listen-Import | Fügt das Feld als Spalte in die Importdatei ein. |
| REST-API | Verwenden Sie die API-Feldnamen `overrideOpenTrackingDefault` und `overrideClickTrackingDefault`. |

Legen Sie jedes Feld entsprechend dem Einverständnis der Person fest. Wenn in Ihrer Einverständnissprache Öffnungen und Klicks separat behandelt werden, konfigurieren Sie jedes Feld unabhängig voneinander.

## Änderungen in der E-Mail

Wenn Marketo Engage beschließt, eine Person nicht nachzuverfolgen, ändert sich der E-Mail-Inhalt, den es an diese Person sendet.

| Tracking für deaktiviert | Änderungen | Was noch funktioniert |
|---|---|---|
| Geöffnet | Die E-Mail enthält nicht das Öffnungs-Tracking-Pixel. Es **keine Aktivität vom Typ** E-Mail öffnen“ aufgezeichnet. | Andere E-Mail-Funktionen, einschließlich Klick-Tracking, sofern aktiviert. |
| Klicks | Links gehen direkt zu ihren Zielen und nicht über die Tracking-Domain von Marketo Engage. Der ausgeblendete Tracking-Link wird nicht hinzugefügt. Es **keine Aktivität vom Typ „E** Mail-Klick“ aufgezeichnet. | Abmelde-Links, der E-Mail-Fußzeilen-Opt-out-Link, `list-unsubscribe` und **Als Web-Seite anzeigen**-Links funktionieren weiterhin. Bei Verwendung dieser Links wird keine Aktivität vom Typ **E-Mail**. |

## Welche E-Mails sind betroffen?

| E-Mail-Typ | Überschreibungen angewendet? |
|---|---|
| Batch-E-Mails, z. B. E-Mails, die von einer Smart-Batch-Kampagne oder einem E-Mail-Programm gesendet werden | Ja |
| Trigger-E-Mails, z. B. E-Mails, die von einer intelligenten Trigger-Kampagne gesendet werden | Ja |
| E-Mails mit A/B-Tests oder Champion-/Challenger-Varianten | Ja. Das Tracking wird für jede Person separat festgelegt, unabhängig von der Variante, die sie erhält. |
| Als Webseite anzeigen | Ja. Die Web-Version folgt den aktuellen Einstellungen der Person. Das Anzeigen einer Änderung kann bis zu einer Stunde dauern. |
| Operative E-Mails | Nein. Sie folgen normalem Tracking-Verhalten. |
| Beispiel-(Test-)E-Mails | Nein. Sie folgen normalem Tracking-Verhalten. |
| E-Mail-Vorschau | Keine Änderung. Vorschauen werden nicht verfolgt. |
| Warn-E-Mails | Keine Änderung. Warnhinweise werden nicht verfolgt. |
| SMS-Nachrichten | Nein. Diese Funktion gilt nur für E-Mails. |

## Wenn Marketo Engage die Tracking-Entscheidung trifft

Marketo Engage liest die Überschreibungswerte einer Person, wenn es die E-Mail für den Versand vorbereitet.

- **Geplanter oder verzögerter Versand:** Wenn eine E-Mail jetzt vorbereitet und zu einem späteren Zeitpunkt zugestellt wird, z. B. mit der Zeitzone „Kopfstart“ oder „Empfänger“, gelten die Werte zur Vorbereitungszeit. Eine nach der Vorbereitung vorgenommene Änderung ändert diese E-Mail nicht.
- **Bereits zugestellte E-Mails:** Ändern der Überschreibung einer Person ändert sich nichts an den E-Mails, die sie bereits erhalten hat. Klicks auf Links in zuvor gesendeten E-Mails können weiterhin verfolgt werden, wenn diese Links mit aktiviertem Tracking vorbereitet wurden.
- **Zukünftige E-Mails:** Eine Änderung gilt für E-Mails, die Marketo Engage nach der Änderung vorbereitet.

Wenn eine Person ihr Einverständnis widerruft, aktualisieren Sie ihren Überschreibungswert so bald wie möglich, sodass die Änderung für die nächste für sie vorbereitete E-Mail gilt.

## Auswirkungen auf Reporting, Smart Lists und Bewertung

Wenn Marketo Engage eine Person nicht verfolgt, werden keine **E-Mail öffnen** oder **E-Mail klicken** für sie aufgezeichnet. Das Ergebnis:

- **Intelligente Kampagnen:** Filter und Trigger wie **Geöffnete E-Mail** und **geklickter Link in E-Mail** stimmen für diese Person nicht überein oder werden nicht ausgelöst, wenn die entsprechende Aktivität nicht verfolgt wird.
- **Berichte und Dashboards:** Öffnungsraten von E-Mails, Klickraten und Link-Performance spiegeln nur verfolgte Personen wider. Interaktionsmetriken können verringert werden, wenn mehr Personen nicht erfasst werden.
- **Bewertung und Programmerfolg:** Regeln und Programmerfolgsschritte, die auf Öffnungen oder Klicks basieren, gelten nicht für Personen, deren Aktivitäten nicht verfolgt werden. Überprüfen Sie diese Regeln, damit Personen nicht auf unfaire Weise bewertet oder weiterentwickelt werden.
- **Web-Aktivitätsverknüpfung:** Ist das Klick-Tracking deaktiviert, tragen E-Mail-Links nicht das Tracking-Token von Marketo Engage. Wenn die Person Munchkin noch nicht bekannt ist, wird ein Website-Besuch aus dieser E-Mail nicht über den Link mit der Person verknüpft.

**Aktivitäten vom Typ „Gesendet“, „Zugestellt“, „Bounce“ und „Abgemeldet“ sind nicht betroffen.**

## Funktionsweise mit anderen Tracking-Einstellungen

E-Mail-Tracking-Überschreibungen auf Personenebene können das Tracking für eine Person deaktivieren. Das Tracking wird nicht aktiviert, wenn es bereits durch eine andere Einstellung deaktiviert wurde. Beispielsweise bleiben mit der `mktNoTrack`-Klasse markierte Links auch dann nicht verfolgt, wenn die Einstellungen der Person ein Klick-Tracking zulassen.

## Funktion deaktivieren

Wenn Adobe die Funktion für Ihre Instanz deaktiviert, kehren die nach der Änderung vorbereiteten E-Mails zum normalen Tracking zurück. Die Überschreibungswerte bleiben in den Personendatensätzen, werden jedoch ignoriert. Wenn die Funktion später wieder aktiviert wird, gelten die gespeicherten Werte erneut.

## Häufig gestellte Fragen

### Kann ich Öffnungen verfolgen, aber keine Klicks für eine Person oder das Gegenteil?

Ja. Das Öffnungs- und Klicktracking wird unabhängig voneinander entschieden. Legen Sie nur das Feld „Überschreiben“ für den Tracking-Typ fest, den Sie ändern möchten.

### Hält mich diese Funktion davon ab, E-Mails an eine Person zu senden?

Nein. Es steuert nur das Tracking. Um den Versand von Marketing-E-Mails an eine Person zu stoppen, verwenden Sie die vorhandenen Funktionen zum Abmelden und Einverständnis .

### Sehen Personen, die nicht verfolgt werden, weiterhin funktionierende Abmelde-Links?

Ja. Abmelde-Links und **Als Web-Seite anzeigen** funktionieren weiterhin für alle Personen.

### Warum hat eine Person, die sich per Opt-out abgemeldet hat, immer noch eine Klick-E-Mail -Aktivität?

Möglicherweise haben sie auf einen Link in einer E-Mail geklickt, die vorbereitet wurde, bevor sich ihr Überschreibungswert geändert hat. Änderungen gelten für E-Mails, die nach der Änderung vorbereitet werden.

### Muss ich meine E-Mail-Vorlagen ändern?

Nein. Marketo Engage wendet die Tracking-Entscheidung bei der Erstellung jeder E-Mail an. Sie müssen Ihre Vorlagen oder E-Mails nicht ändern.

## Verwandte Artikel

- Funktionsweise von E-Mails
- Schritt „Datenflusswert ändern“
- Tracking für einen Link in einer E-Mail deaktivieren
- Vorsprung
- Zeitzone des Empfängers
- E-Mail-Leistungsbericht
