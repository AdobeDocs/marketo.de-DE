---
description: Erfahren Sie, wie C2PA-Metadaten automatisch an KI-generierte Bilder in Marketo Engage angehängt, bei der Bearbeitung beibehalten und für die Herkunft von Inhalten verwendet werden.
title: C2PA-Metadaten in Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 77c4c0b6438f8a5070fd33412b7037b79f7fded1
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 3%

---

# C2PA-Metadaten in Marketo Engage

Im Bereich der generativen KI-Transparenz entstehen neue Gesetze, und Adobe arbeitet daran, die geltenden Anforderungen in allen Rechtssystemen zu erfüllen. C2PA-Metadaten sind das Herkunftstool, das Adobe verwendet, um die Anforderungen dieser Gesetze zu erfüllen.

C2PA-Metadaten sind dauerhafte, unsichtbare Metadaten, die aufzeichnen, wie ein Inhaltselement erstellt oder bearbeitet wurde. Wenn Sie ein Bild mit Tools für generative KI in Marketo Engage generieren oder bearbeiten, werden C2PA-Metadaten automatisch an dieses Bild angehängt (Ihrerseits ist keine Aktion erforderlich). Es handelt sich um verschlüsselte, manipulationssichere Informationen, die Betrachtern helfen können, die Herkunft der Inhalte zu verstehen und die Integrität der Marken-Assets sicherzustellen. Zu diesen Informationen gehören:

* **Aussteller oder Unterzeichner**: Informationen über die Entität oder das Unternehmen, die bzw. das die digitale Signatur zum Zertifizieren oder Signieren des Assets ausgestellt hat.
* **Ausstellungsdatum**: Das Datum, an dem die C2PA-Metadaten auf das Asset angewendet wurden.
* **Gutschrift und Nutzung**: Informationen zum Produzenten des Assets, einschließlich Name, Social-Media-Handles oder anderer identitätsbezogener Informationen.
* **Prozess**: Aufzeichnung aller Bearbeitungen oder Änderungen am Asset.
* **Gerätedetails**: Informationen über die Anwendung oder das Gerät, die bzw. das zum Erstellen oder Bearbeiten des Assets verwendet wird.
* **KI-Tool verwendet**: Wenn die generative KI zum Erstellen des Assets verwendet wurde, kann der Name des verwendeten Modells einbezogen werden.
* **Weitere relevante Informationen**: Es sind auch zusätzliche Daten enthalten, um mehr Kontext über den Verlauf eines Assets anzubieten.

## Aktionen, die C2PA-Metadaten anhängen

In der folgenden Tabelle wird basierend auf der Bildaktion, die bei der Bildgenerierung in Marketo Engage ausgeführt wurde, zusammengefasst, wann C2PA-Metadaten angehängt werden.

| Aktion | Beschreibung | C2PA-Metadaten angehängt? | Anwendungsbeispiel |
|---|---|---|---|
| **Verwenden des Tools „Bild generieren“** | Erstellen Sie ein neues Bild aus einer Textaufforderung, aus einem Referenzbild oder generieren Sie ein ähnliches Bild. | Immer. Das Bild wird durch generative KI generiert, sodass es immer neue C2PA-Metadaten enthält. | Aus einer Textaufforderung, die das gewünschte visuelle Element beschreibt, wird ein Bannerbild für eine E-Mail-Kampagne generiert. |
| **Beschneiden eines Bildes** | Passen Sie ein Bild an die gewünschten Abmessungen an. | Nur wenn das Quellbild bereits C2PA-Metadaten enthielt. Beim Zuschneiden werden die Pixel des Bildes neu erstellt, die normalerweise diese C2PA-Metadaten löschen würden. Daher liest Marketo Engage sie vor dem Zuschneiden aus dem Quellbild, erstellt sie dann neu und fügt sie erneut an das zugeschnittene Ergebnis an. Beim Zuschneiden selbst wird keine neue generative KI-Aktion hinzugefügt, sondern die vorhandene beibehalten. | Ein generiertes Bannerbild wird zugeschnitten, damit es in eine Web-Seite passt: Die C2PA-Metadaten werden durch den Zuschnitt beibehalten. Ein hochgeladenes Stockfoto, das als Hintergrund für eine Push-Benachrichtigung verwendet wird, wird dem Bildschirm zugeordnet: Da das Stockfoto keine generative KI-Aktion aufweist, werden keine C2PA-Metadaten erstellt. |
| **Hinzufügen einer Textüberlagerung** | Generierten Text über einem Hintergrundbild rendern | Nur wenn das Hintergrundbild bereits C2PA-Metadaten enthielt. Beim Rendern der Überlagerung wird ein neues Bild aus dem Hintergrund plus Text erstellt, der diese C2PA-Metadaten normalerweise löscht. Daher liest Marketo Engage es zuvor aus dem Hintergrundbild, erstellt es dann neu und fügt es erneut an das Ergebnis an. Der Überlagerungsschritt fügt keine neue generative KI-Aktion hinzu. | Eine Werbe-Überschrift wird als Textüberlagerung auf einem generierten Hintergrundbild für eine Landingpage gerendert: Die C2PA-Metadaten aus dem Hintergrundbild werden beibehalten. |

## Inhaltstypen und ihr Umfang

**Bilder**: Überdeckt. C2PA-Metadaten werden angehängt, wenn Bilder mit generativer KI generiert werden, und bleiben durch Zuschneiden und Textüberlagerung erhalten, die von der Bildgenerierung in Marketo Engage ausgeführt werden.

**Text**: Nicht zutreffend. Reine Textausgaben der Bilderstellung in Marketo Engage, z. B. Kopiergenerierung, Übersetzung und Vorschläge für die Markenausrichtung, erfordern keine C2PA-Metadaten.

## Was passiert, wenn Inhalte verschoben werden?

Marketo Engage behält C2PA-Metadaten bei, die mit unterstützten Bild-Assets verknüpft sind. Wenn ein Bild beim Import in Marketo Engage C2PA-Metadaten enthält, werden die Metadaten beibehalten, wenn das Asset in generierten Kampagneninhalten und in ausgehenden E-Mail-Erlebnissen verwendet wird.

## Zusätzliche Ressourcen

* [Benutzerrichtlinien für die generative KI von Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* [Leitlinien und Einschränkungen](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails)
