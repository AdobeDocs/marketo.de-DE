---
description: Die Beschreibung ist hier zu finden.
title: Organisationsregeln
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%
---
# Organisationsregeln {#organizational-rules}

Organisatorische Regeln definieren Ihre Marketing-Betriebsstandards und Governance-Anforderungen in einem einzigen Dokument, das Kollegen über die Programmerstellung, Kampagnenplanung und Validierungs-Workflows hinweg leitet.

## Was sind Organisationsregeln? {#what-are-organizational-rules}

Organisationsregeln sind ein Markdown-basiertes Konfigurationsdokument, das die Kampagnenstandards Ihres Unternehmens erfasst:

* Benennungskonventionen für Programme, E-Mails und Smart-Kampagnen
* Erforderliche Assets und Struktur (Ordner, Token, Berichte)
* Compliance-Anforderungen (Abmelde-Links, UTM-Parameter, Ausschlussfilter)
* Best Practices (E-Mail-Design, Smart-Listen-Konfiguration)

Jede Marketo-Instanz enthält standardmäßige Organisationsregeln. Sie können sie an die spezifischen Governance-Anforderungen Ihres Unternehmens anpassen.

## Wo Organisationsregeln verwendet werden {#where-organizational-rules-are-used}

Organisatorische Regeln führen Coworker durch drei Fähigkeiten:

| Skill | So werden Regeln angewendet |
| --- | --- |
| Erstellen von Programmen | Regeln dienen zur Erstellung der Programmstruktur, Benennung und Ersteinrichtung. Mitarbeiter kennzeichnet alle Compliance-Probleme in Ihrer Zusammenfassung, bevor Sie das Programm erstellen. |
| Kampagnen planen | Die Regeln bestimmen, wie Mitarbeiter intelligente Kampagnen, Filter und Flussschritte basierend auf Ihren Standards strukturieren. |
| Programme validieren | Regeln definieren, was von einem Mitarbeiter vor der Aktivierung bei der Validierung von Programmen überprüft wird. |

## Zugriff auf und Anpassung von Organisationsregeln {#how-to-access-and-customize-organizational-rules}

1. Klicken Sie in My Marketo auf die Kachel **Mitarbeiter für Marketo Engage**.
1. Klicken Sie auf das Zahnradsymbol.
1. Wählen Sie die **Organisationsregeln** aus.
1. Überprüfen Sie die Standardregeln (diese enthalten bereits Best Practices für Marketing-Vorgänge).
1. Bearbeiten Sie die Regeln so, dass sie den Ihrer Organisation entsprechen:

   * Benennungskonventionen (Programme, E-Mails, Kampagnen)
   * Erforderliche Ordnerstruktur
   * Erforderliche Token und Felder
   * Konformitäts- und Ausschlussstandards

1. Versionsnummer bei Änderungen aktualisieren
1. Speichern Sie Ihre Änderungen. Alle Mitarbeiter-Fähigkeiten verwenden sofort Ihre benutzerdefinierten Regeln.

## Struktur der Organisationsregeln {#organizational-rules-structure}

Organisationsregeln werden in Markdown mit YAML-Schriftart formatiert:

```markdown
---
name: Your Organization Name — Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## ⚠️ REQUIRED Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## Best Practices für Organisationsregeln {#best-practices-for-organizational-rules}

* **Mit Standardwerten beginnen**: Überprüfen Sie die Standardregeln, bevor Sie sie anpassen. Sie spiegeln branchenspezifische Best Practices für Marketing-Vorgänge wider.
* **Regeln fokussieren**: Schließen Sie nur Anforderungen ein, die für Ihr Unternehmen wichtig sind. Unnötige Regeln verursachen Lärm und verringern unnötige Compliance-Bewertungen.
* **Verwenden Sie sowohl automatisierte als auch manuelle Prüfungen**:

  * Automatisierte Prüfungen - Namenskonventionen, erforderliche Ordner, Token-Nutzung (kann von Kollegen überprüft werden)
  * Manuelle Prüfungen - visuelles Design von E-Mails, Markenkonformität, Kampagnenlogik (Coworker kennzeichnet diese als manuelle Überprüfungsschritte)

* **Schärfe mit Flexibilität in Einklang bringen**: Zu strenge Regeln können die Programmerstellung verlangsamen. Zu lockere Regeln lösen keine wichtigen Compliance-Probleme aus.
* **Ihre Regeln versionieren**: Aktualisieren Sie die Versionsnummer, wenn Sie wichtige Änderungen vornehmen, damit Ihr Team weiß, dass die Governance-Standards aktualisiert wurden.
* **Änderungen mitteilen**: Wenn Sie Organisationsregeln aktualisieren, informieren Sie Ihr Marketing-Opportunity-Team darüber, was sich geändert hat und warum.

## Was ein Kollege validieren kann und was nicht {#what-coworker-can-and-cannot-validate}

Mitarbeiter KANN validieren (automatisierte Prüfungen):

* Benennungskonventionen entsprechen Ihren Mustern
* Erforderliche Ordnerstruktur vorhanden
* Erforderliche Token sind vorhanden
* E-Mail enthält einen Abmelde-Link und die erforderlichen Fußzeilenelemente
* Externe Links enthalten UTM-Parameter
* Namen intelligenter Kampagnen folgen Konventionen

Worker kann nicht validieren (manuelle Überprüfung erforderlich):

* Logik des Smart List-Filters (API-Einschränkung - Filter müssen manuell konfiguriert werden)
* Logik der Schritte für intelligente Kampagnenflüsse (API-Einschränkung - Flüsse müssen manuell konfiguriert werden)
* Visuelles Rendering und Reaktionsfähigkeit von E-Mails (erfordert visuelle Überprüfung)
* Markenkonformität und Aussagekraft (erfordert menschliches Urteilsvermögen)
* Segmentierungsregeln für dynamische Inhalte (API-Einschränkung)

Wenn ein Mitarbeiter auf etwas stößt, das nicht validiert werden kann, wird es als manueller Überprüfungsschritt im Workflow gekennzeichnet.

## Compliance Scoring {#compliance-scoring}

Wenn Sie „Programme validieren“ verwenden, berechnet Coworker einen Compliance-Score auf Basis von:

* **Prüfungen bestanden** - Mitarbeiter hat die Einhaltung der Vorgaben überprüft und keine Probleme gefunden
* **Fehlgeschlagene Prüfungen** - Mitarbeiter hat Verstöße gegen Ihre Organisationsregeln gefunden
* **Manuelle Überprüfungsschritte** - Elemente, für die eine menschliche Überprüfung erforderlich ist (diese werden NICHT gegen Ihre Bewertung gezählt)

Ein Programm kann zu 100 % konform sein und erfordert weiterhin manuelle Überprüfungsschritte - sie werden aus der Score-Berechnung ausgeschlossen.

## Beispiele für die Anpassung von Organisationsregeln {#examples-of-organizational-rules-customization}

**Beispiel 1: Strenge Namenskonvention**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

Verwenden Sie dies, wenn Ihr Unternehmen eine strikte Governance für alle Regionen und Geschäftsbereiche erfordert.

**Beispiel 2: Flexible Benennung mit erforderlichem Präfix**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

Verwenden Sie diese Option, wenn Sie Konsistenz bei Regions-Codes, aber Flexibilität bei den übrigen Codes wünschen.

**Beispiel 3: Minimale Regeln (Fokus auf Compliance)**

```markdown
# Email Compliance — REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

Verwenden Sie diese Option, wenn Ihr Unternehmen der Compliance Vorrang vor der Benennung/Strukturkonsistenz einräumt.

## Fehlerbehebung {#troubleshooting}

**F: Ich habe die Organisationsregeln aktualisiert, aber die Mitarbeiter verwenden weiterhin die alten Regeln.**

A.: Änderungen treten bei neuen Programmen und Validierungen sofort in Kraft. Wenn Sie an einem vorhandenen Programm arbeiten, aktualisieren Sie Ihren Browser oder starten Sie einen neuen Kollegen-Workflow, um die aktualisierten Regeln anzuzeigen.

**F: Kann ich zu Standardregeln zurückkehren?**

A: Ja. Wechseln Sie zu **Einstellungen** > **Organisationsregeln** und klicken Sie auf **Auf Standard zurücksetzen**. Die benutzerdefinierten Regeln werden durch die Standardregeln ersetzt.

**F: Meine Compliance-Bewertung ist niedrig, obwohl das Programm gut aussieht.**

A: Überprüfen Sie, welche Prüfungen fehlschlagen. Überprüfen Sie Ihre Organisationsregeln, um festzustellen, ob sie für Ihre aktuellen Workflows zu streng sind oder ob Sie das Programm an Ihre Standards anpassen müssen.
