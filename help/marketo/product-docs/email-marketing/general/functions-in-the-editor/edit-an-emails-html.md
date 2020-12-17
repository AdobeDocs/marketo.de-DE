---
unique-page-id: 1900554
description: Bearbeiten des HTML-Codes einer E-Mail - Marketing-Dokumente - Produktdokumentation
title: HTML einer E-Mail bearbeiten
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Bearbeiten von HTML einer E-Mail {#edit-an-emails-html}

Manchmal müssen Sie die zugrunde liegende HTML einer E-Mail ändern. Manchmal kann ein externes System zum Entwerfen und Erstellen des E-Mail-Codes verwendet werden. Sie können Code ganz einfach aus dem E-Mail-Editor importieren und/oder bearbeiten.

## HTML bearbeiten {#edit-html}

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/teamspidey.jpg)

1. Klicken Sie auf **Code bearbeiten**.

   ![](assets/two-4.png)

1. Nehmen Sie alle Änderungen vor. Klicken Sie abschließend auf **Speichern**.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Ändere, was du willst. Sie können das gesamte HTML ersetzen oder kleinere Anpassungen vornehmen.

1. Klicken Sie auf die Dropdown-Liste **Code-Aktionen**, um den Code als HTML-Datei herunterzuladen, Ihre CSS zu inline oder die HTML zu validieren.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >Die beste Methode für E-Mails ist, alle Stile inline zu gestalten. Mehrere E-Mail-Clients unterstützen CSS im Abschnitt `<head>` nicht.

## Aufbrechen einer E-Mail aus ihrer Vorlage {#breaking-an-email-from-its-template}

Diese Codeänderungen **unterbrechen eine E-Mail nicht aus ihrer Vorlage:**

* Bearbeiten des Inhalts eines Moduls (einschließlich des Hinzufügens neuer Elemente innerhalb des Moduls)
* Hinzufügen eines neuen Moduls zum Container
* Löschen eines Moduls vom Container

* Ändern von kto-spezifischen Attributen (z. B. &quot;mktoName&quot;oder &quot;mktoImgUrl&quot;) eines Elements außerhalb eines Moduls
* Bearbeiten des Inhalts eines Elements (Rich Text, Bild, Video usw.) außerhalb eines Moduls

Die folgenden Schritte können Sie im Code-Editor **durchführen, um die E-Mail aus der Vorlage zu entfernen:**

* Ändern von Elementen im Code außerhalb eines Elements oder Moduls
* Hinzufügen oder Ändern von Nicht-mkto-Attributen (z. B. &quot;id&quot;oder &quot;style&quot;) eines Elements außerhalb eines Moduls
* Löschen eines Elements außerhalb eines Moduls

## Suchcode {#search-code}

Verwenden Sie die Funktion &quot;Suchcode&quot;, um Inhalte im HTML-Code Ihrer E-Mail effizient zu finden und zu ersetzen.

1. Klicken Sie im Code Ihrer E-Mail auf **Suchcode**.

   ![](assets/five-2.png)

1. Geben Sie an, was Sie suchen möchten, und klicken Sie auf **Weitersuchen**, um vorwärts zu suchen, oder auf **Vorherige suchen**, um rückwärts zu suchen. Sie haben auch die Option **Ersetzen** und **Alle ersetzen**.

   ![](assets/six-1.png)

1. Klicken Sie abschließend auf **Schließen**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Der Suchcode ist auch im Editor [E-Mail-Vorlage](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template) verfügbar.

Es wird empfohlen, dass Sie Ihre E-Mails weiterhin mit der integrierten Funktionalität von Marketo bearbeiten. Dieser Code-Editor bietet jedoch Flexibilität, wenn Sie ihn benötigen.
