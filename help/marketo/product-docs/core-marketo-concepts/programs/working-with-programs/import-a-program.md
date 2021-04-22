---
unique-page-id: 1147108
description: Programm importieren - Marketo Docs - Produktdokumentation
title: Programm importieren
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Programm {#import-a-program} importieren

Ein Programm kann von einem Marketo-Abonnement in ein anderes importiert werden. Sie können beispielsweise ein Programm in einer Sandbox erstellen und es dann in Ihr Live-Abonnement importieren. Außerdem können Sie ein vordefiniertes Programm aus der Marketo Programm Library importieren.

## Programm {#import-a-program-1} importieren

1. Gehen Sie zu **Marketing-Aktivitäten.**

   ![](assets/ma.png)

1. Klicken Sie auf die Dropdownliste **Neu**. Wählen Sie **Programm importieren**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >Programm Import ist nur für Benutzer verfügbar, für die die Berechtigung Programm importieren aktiviert ist. Erfahren Sie mehr über [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Um ein Sandbox-Konto mit Ihrem Live-Abonnement zu verbinden, wenden Sie sich an den [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Wählen Sie ein Marketo **Abonnement** und ein zu importierendes Programm aus. Klicken Sie auf **Weiter**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Geben Sie einen **Kampagne-Ordner** für das importierte Programm an. Klicken Sie auf **Weiter.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Vergewissern Sie sich, dass **Standardkonflikt**-Regeln verwenden ausgewählt ist. Konfliktregeln sind erforderlich, wenn Sie Programm in eine Instanz importieren, deren Assets denselben Namen haben.

1. Details zur Vorschau und **Importieren** des Programms.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   In einem Dialogfeld wird der Fortschritt beim Importieren des Programms angezeigt.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Sobald der Import abgeschlossen ist, erhalten Sie eine E-Mail-Bestätigung.

>[!NOTE]
>
>Sie müssen importierte Batch-Kampagnen neu planen und Trigger-Kampagnen aktivieren. Das System deaktiviert automatisch die Kampagnen für die Kampagne und den Trigger im importierten Programm.

## Identifizieren Sie vorab erstellte Programm in der Marketo-Programm-Bibliothek {#identify-pre-built-programs-in-the-marketo-program-library}

Die Marketo Programm Library enthält vordefinierte, getestete Programm, die Sie in Ihr Abonnement importieren können. Zu den verfügbaren Programmen gehören:

1. **Grundlegende Drip Nurture.** Sendet eine Reihe von E-Mails getrennt durch Warteschritte.
1. **Datenverwaltung.** Behält die Datenintegrität mithilfe intelligenter Kampagnen bei.
1. **E-Mail mit Landingpage.** Sendet eine erste E-Mail mit einem Angebot, z. B. &quot;Dieses Whitepaper herunterladen&quot;. Fügt eine Bestätigungs- oder Erinnerungsmail hinzu. Beinhaltet eine Landingpage mit einem Formular.
1. **E-Mail mit Fortschrittsstatus.** Sendet eine Mail-Nachricht mit einem nachverfolgbaren Link, auf den die Person klicken kann. Aktualisiert den Status der Progression für jede Person - Gesendet, Geöffnet, angeklickt usw.
1. **Interessante Momente.** Erstellt interessante Momente für Ihr Verkaufsteam, um sie in der Schleife zu halten.
1. **Landingpage mit Autoresponder.** Verwenden Sie herunterladbare Inhalte, um neue Leute zu gewinnen und sie zu fördern. Umfasst Landingpages und Formulare.
1. **Lebenszyklus 2.** Verwendet Scoring, um eine Person von neu zu marketingfähig zu bewegen.
1. **Mobile E-Mail-Vorlage.** Eine reaktionsfähige E-Mail-Vorlage, die mit iPhone und Android getestet wurde. Bestimmte Versionen von Android-, MS Outlook-, Exchange- und Drittanbieter-Apps wie Gmail und Yahoo! Mobile Mail-Apps unterstützen kein CSS, das für reaktionsfähige Vorlagen erforderlich ist. Wir empfehlen Ihnen, vor dem Versenden von E-Mails einen Test durchzuführen.
1. **Preisausschreiben beim Programm importieren.** Preisausschreiben Programm für diejenigen, die die Programm-Bibliothek ausprobieren! Genehmigen Sie einfach die E-Mails und die Landingpage und aktivieren Sie die intelligente Kampagne. Dann Ansicht die genehmigte Landingpage, füllen Sie das Formular aus und Sie werden eingegeben!
1. **Verfügbare Kampagnen zum Verkauf** Bietet Ihren Vertriebsmitarbeitern eine Möglichkeit, Marketo Smart-Kampagnen aus einem Dashboard in Ihrem CRM auszuführen.
1. **Scoring - Spark Edition.** Demografische Bewertung und Verhaltens, die in einem einzigen Bewertungsfeld erfasst werden. Umfasst mehr als zwei Dutzend Kampagnen, die mit Scoring zusammenhängen.
1. **Bewertung - Standard- und Select-Editionen.** Demografische Bewertung und Verhaltens, die in separaten Bewertungsfeldern erfasst werden. Umfasst mehr als zwei Dutzend Kampagnen, die mit Scoring zusammenhängen.
1. **Synchronisieren Sie Neue Personen mit CRM.** Die Kampagne, die neue Leute mit Ihrem CRM-System synchronisiert. Er weist einem Personenstand den Status zu, dass er als nicht verkaufsbereit anerkannt wird.
1. **Webinar mit Ereignis Adapter.** Eine ganze Reihe von E-Mails - wie Einladungen und Erinnerungen - sowie Landingpages mit Formularen und Kampagnen, um Menschen durch das Programm zu bewegen. In diesem Programm erhalten Sie aktuelle Informationen zur Registrierung, zur Teilnahme usw. von Online-Ereignissen wie WebEx.
1. **Webinar ohne Ereignis-Adapter.** Wie oben, aber mit manuellen Prozessen zur Registrierung, Anwesenheitskontrolle, etc.
1. **Sirius entscheidet Scoring Programm**. Dieses Programm wurde entwickelt, um das Sirius Decision Scoring-Standardmodell zu unterstützen, einschließlich der impliziten und expliziten Bewertungsregeln und der Zuweisung von Matrixpersonen.

>[!CAUTION]
>
>Sie müssen zwei benutzerdefinierte Felder (&quot;Demografische Bewertung&quot;und &quot;Verhaltensbewertung&quot;) erstellen, bevor Sie das Programm &quot;Bewertung - Standard- und Auswahl-Editionen&quot;importieren.

## Auswirkungen auf externe Assets bei Programm-Importen {#impact-on-external-assets-during-program-imports}

Programme verwenden externe Assets wie E-Mail-Vorlagen, Vorlagen für Landingpages, Bilder, Formulare, Token und Programm-Tags. Sie können konfigurieren, wie Landingpages- und Programm-Tags verarbeitet werden, und Marketo verwaltet den Rest automatisch.

**E-Mail-Vorlagen:** E-Mail-Vorlagen werden automatisch importiert und erstellt, es sei denn, eine Vorlage mit demselben Namen ist vorhanden.

**Vorlagen für Landingpages: Vorlagen für** Landingpages werden in das Design-Studio importiert. Mithilfe von Konfliktregeln können Sie das Verhalten konfigurieren, wenn eine Vorlage mit demselben Namen vorhanden ist. Bei Verwendung der Standardregel wird eine Landingpage an eine Vorlage angehängt, wenn eine mit demselben Namen vorhanden ist. Eine Vorlage mit dem Namen &quot;Standardvorlage 1&quot;wird beispielsweise erstellt, wenn eine Landingpage mit dem Namen &quot;Standardvorlage&quot;vorhanden ist.

**Bilder:** Von Landingpages verwendete Bilder werden in das Design-Studio importiert, es sei denn, es ist eines mit demselben Namen vorhanden.

**Token:** Token, die außerhalb eines Programms leben, werden während des Importvorgangs in lokale Token konvertiert.

>[!CAUTION]
>
>Bildtyp, den meine Token für Programm-Importe nicht unterstützen. Wenn ein Programm mit meinem Token importiert wird, werden **keine** Token angezeigt.

**Programm-Tags:** Sie können mit Konfliktregeln steuern, wie Programm-Tags, die nicht im Zielkonto vorhanden sind, behandelt werden. Mithilfe der Standardregel werden die Programm-Tags erstellt oder Sie können die Tags ignorieren. **Forms:** Externe Formulare werden automatisch in das Design-Studio importiert, es sei denn, es ist ein gleichnamiges Formular vorhanden.

>[!CAUTION]
>
>Beim Importieren eines Programms werden Landingpages/E-Mails, die [dynamische Inhalte](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) enthalten, übersprungen.
