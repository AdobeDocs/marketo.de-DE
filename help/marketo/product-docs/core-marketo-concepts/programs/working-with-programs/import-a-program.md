---
unique-page-id: 1147108
description: Programm importieren - Marketo-Dokumente - Produktdokumentation
title: Programm importieren
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Programm importieren {#import-a-program}

Ein Programm kann aus einem Marketo-Abonnement in ein anderes importiert werden. Sie können beispielsweise ein Programm in einer Sandbox erstellen und es dann in Ihr Live-Abonnement importieren. Außerdem können Sie ein vordefiniertes Programm aus der Marketo-Programmbibliothek importieren.

## Programm importieren {#import-a-program-1}

1. Gehen Sie zu **Marketingaktivitäten.**

   ![](assets/ma.png)

1. Klicken Sie auf die Dropdown-Liste **Neu** . Wählen Sie **Programm importieren** aus.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >Der Programm-Import ist nur für Benutzer verfügbar, deren Rollen mit der Berechtigung Programm importieren aktiviert sind. Erfahren Sie mehr über [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Um ein Sandbox-Konto mit Ihrem Live-Abonnement zu verbinden, wenden Sie sich an [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Wählen Sie eine Marketo **Subscription** und ein zu importierendes Programm aus. Klicken Sie auf **Next**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Geben Sie einen **Kampagnenordner** für das importierte Programm an. Klicken Sie auf **Weiter.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass **Standardkonfliktregeln** ausgewählt sind. Konfliktregeln sind erforderlich, wenn Sie Programme in eine Instanz importieren, die Assets mit demselben Namen enthält.

1. Vorschau der Details und **Import** des Programms.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Ein Dialogfeld zeigt den Fortschritt des Programmimports an.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Sie erhalten eine E-Mail-Bestätigung, sobald der Import abgeschlossen ist.

>[!NOTE]
>
>Sie müssen importierte Batch-Kampagnen neu planen und Trigger-Kampagnen aktivieren. Das System deaktiviert automatisch Kampagnenzeitpläne und Trigger-Kampagnen im importierten Programm.

## Ermitteln von vordefinierten Programmen in der Marketo-Programmbibliothek {#identify-pre-built-programs-in-the-marketo-program-library}

Die Marketo-Programmbibliothek enthält vordefinierte, getestete Programme, die Sie in Ihr Abonnement importieren können. Zu den verfügbaren Programmen gehören:

1. **Grundlegende Treibstoffzufuhr.** Sendet eine Reihe von E-Mails, getrennt durch Warteschritte.
1. **Datenverwaltung.** Die Datenintegrität wird mithilfe von Smart-Kampagnen verwaltet.
1. **E-Mail mit Landingpage.** Sendet eine erste E-Mail mit einem Angebot, z. B. &quot;Dieses Whitepaper herunterladen&quot;. Fügt eine Bestätigungs- oder Erinnerungsmail hinzu. Enthält eine Landingpage mit einem Formular.
1. **E-Mail mit Fortschrittsstatus.** Sendet eine E-Mail-Nachricht mit einem trackbaren Link, auf den die Person klicken kann. Aktualisiert den Fortschritt für jede Person - Gesendet, Geöffnet, Angeklickt usw.
1. **Interessante Momente.** Erstellt interessante Momente für Ihr Verkaufsteam, um sie in der Schleife zu halten.
1. **Landingpage mit Autoresponder.** Verwenden Sie herunterladbare Inhalte, um neue Personen zu gewinnen und sie zu pflegen. Umfasst Landingpages und Formulare.
1. **Lebenszyklus 2.** Verwendet Scoring, um eine Person von einer neuen in eine Marketing qualifizierte zu verschieben.
1. **Mobile E-Mail-Vorlage.** Eine responsive E-Mail-Vorlage, die mit iPhone und Android getestet wurde. Bestimmte Versionen von Android-, MS Outlook-, Exchange- und Drittanbieter-Apps wie Gmail und Yahoo! Mobile E-Mail-Apps unterstützen nicht das für responsive Vorlagen erforderliche CSS. Wir empfehlen Ihnen, vor dem Versand von E-Mails einen Test durchzuführen.
1. **Preisausschreiben beim Programmimport.** Preisausschreiben für diejenigen, die die Programmbibliothek ausprobieren! Validieren Sie einfach die E-Mails und die Landingpage und aktivieren Sie die Smart-Kampagne. Dann sehen Sie sich die genehmigte Landingpage an, füllen Sie das Formular aus und Sie werden eingetragen!
1. **Verfügbare Kampagnen für Verkäufe.** Bietet Ihren Vertriebsmitarbeitern die Möglichkeit, Smart-Kampagnen aus Marketo über ein Dashboard in Ihrem CRM-System auszuführen.
1. **Scoring - Spark Edition.** Demografische und verhaltensbasierte Bewertung, die in einem einzigen Scoring-Feld erfasst werden. Umfasst mehr als zwei Dutzend Scoring-bezogene Kampagnen.
1. **Scoring - Standardbearbeitung und Auswahl von Editionen.** Demografische und verhaltensbezogene Bewertung, die in separaten Scoring-Feldern erfasst wird. Umfasst mehr als zwei Dutzend Scoring-bezogene Kampagnen.
1. **Synchronisieren neuer Personen mit CRM.** Die Kampagne, die neue Personen mit Ihrem CRM-System synchronisiert. Er weist einen Personenstand so zu, dass er als nicht verkaufsbereit erkannt wird.
1. **Webinar mit Ereignisadapter.** Eine vollständige Reihe von E-Mails - wie z. B. Einladungen und Erinnerungen - sowie Landingpages mit Formularen und Kampagnen, um Personen durch das Programm zu bewegen. Dieses Programm enthält aktuelle Informationen über Registrierung, Teilnahme usw. von Online-Ereignisanbietern wie WebEx.
1. **Webinar ohne Ereignisadapter.** Wie oben, aber mit manuellen Prozessen für die Registrierung, Anwesenheit, usw.
1. **Scoring-Programm für Sirius-Entscheidungen**. Dieses Programm unterstützt das Standard-Scoring-Modell für Sirius-Entscheidungen, einschließlich der impliziten und expliziten Scoring-Regeln und der Zuweisung von matrixten Personen.

>[!CAUTION]
>
>Vor dem Import des Programms Scoring - Standard &amp; Select Editions müssen Sie zwei benutzerdefinierte Felder (&quot;Demografische Punktzahl&quot;und &quot;Verhaltensbewertung&quot;) erstellen.

## Auswirkungen auf externe Assets bei Programmeinfuhren {#impact-on-external-assets-during-program-imports}

Programme verwenden externe Assets wie E-Mail-Vorlagen, Landingpage-Vorlagen, Bilder, Formulare, Token und Programm-Tags. Sie können konfigurieren, wie Landingpage-Vorlagen und Programm-Tags verarbeitet werden, und Marketo verwaltet den Rest automatisch.

**E-Mail-Vorlagen:** E-Mail-Vorlagen werden automatisch importiert und erstellt, es sei denn, eine Vorlage mit demselben Namen ist vorhanden.

**Landingpage-Vorlagen:** Landingpage-Vorlagen werden in das Design-Studio importiert. Sie können Konfliktregeln verwenden, um das Verhalten zu konfigurieren, wenn eine Vorlage mit demselben Namen vorhanden ist. Unter Verwendung der Standardregel wird eine Zahl an eine Landingpage-Vorlage angehängt, wenn eine mit demselben Namen vorhanden ist. Beispielsweise wird eine Landingpage-Vorlage mit dem Namen Standardvorlage 1 erstellt, wenn eine mit dem Namen Standardvorlage vorhanden ist.

**Bilder:** Von Landingpages verwendete Bilder werden in das Design-Studio importiert, es sei denn, es existiert eines mit demselben Namen.

**Token:** Token, die außerhalb eines Programms liegen, werden während des Importvorgangs in lokale Token konvertiert.

>[!CAUTION]
>
>Bildtyp Meine Token werden für Programmimporte nicht unterstützt. Wenn ein Programm importiert wird, das den Bildtyp meiner Token aufweist, werden **no** Token angezeigt.

**Programm-Tags:** Sie können Konfliktregeln verwenden, um zu steuern, wie Programm-Tags, die im Zielkonto nicht vorhanden sind, behandelt werden. Durch die Verwendung der Standardregel werden die Programm-Tags erstellt, oder Sie können die Tags ignorieren.

**Forms:** Externe Formulare werden automatisch in das Design-Studio importiert, es sei denn, es existiert ein Formular mit demselben Namen.

>[!CAUTION]
>
>Beim Importieren eines Programms werden Landingpages/E-Mails, die [dynamische Inhalte](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) enthalten, übersprungen.
