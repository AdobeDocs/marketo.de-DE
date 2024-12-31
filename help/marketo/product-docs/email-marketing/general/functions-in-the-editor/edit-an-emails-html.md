---
unique-page-id: 1900554
description: E-Mail-HTML bearbeiten - Marketo-Dokumente - Produktdokumentation
title: HTML einer E-Mail bearbeiten
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# HTML einer E-Mail bearbeiten {#edit-an-emails-html}

Manchmal muss der zugrunde liegende HTML einer E-Mail geändert werden. Manchmal können Sie ein externes System verwenden, um den Code Ihrer E-Mail zu entwerfen und zu erstellen. In beiden Fällen können Sie Code einfach aus dem E-Mail-Editor importieren und/oder bearbeiten.

## HTML bearbeiten {#edit-html}

1. Wählen Sie Ihre E-Mail aus und klicken Sie **Entwurf bearbeiten**.

   ![](assets/teamspidey.jpg)

1. Klicken Sie **Code bearbeiten**.

   ![](assets/two-4.png)

1. Nehmen Sie beliebige Änderungen vor. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Ändere, was du willst. Sie können die gesamte HTML austauschen oder kleinere Anpassungen vornehmen.

1. Klicken Sie auf die **Code-Aktionen**, um den Code als HTML-Datei herunterzuladen, Ihre CSS-Datei inline zu erstellen oder die HTML zu validieren.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >Die Best Practice für E-Mails besteht darin, alle Stile inline zu erstellen. Mehrere E-Mail-Clients unterstützen CSS im `<head>` nicht.

## E-Mails aus Vorlagen umbrechen {#breaking-an-email-from-its-template}

Durch diese Code **Änderungen wird** E-Mail aus ihrer Vorlage beschädigt:

* Bearbeiten des Inhalts eines beliebigen Moduls (einschließlich des Hinzufügens neuer Elemente innerhalb des Moduls)
* Hinzufügen eines neuen Moduls zum Container
* Löschen eines Moduls aus dem Container

* Ändern von mkto-spezifischen Attributen (z. B. „mktoName“ oder „mktoImgUrl„) eines beliebigen Elements außerhalb eines Moduls
* Bearbeiten des Inhalts eines beliebigen Elements (Rich-Text, Bild, Video usw.) außerhalb eines Moduls

Diese Aktionen, die Sie im Code-Editor durchführen können **unterbrechen** E-Mail in ihrer Vorlage:

* Ändern von Elementen im Code außerhalb eines Elements oder Moduls
* Hinzufügen oder Ändern von Nicht-Moto-Attributen (z. B. „id“ oder „style„) von beliebigen Elementen außerhalb eines Moduls
* Löschen eines Elements, das sich außerhalb eines Moduls befindet

## Code suchen {#search-code}

Verwenden Sie die Suchcodefunktion, um Inhalte im HTML-Code Ihrer E-Mail effizient zu finden und zu ersetzen.

1. Klicken Sie im Code Ihrer E-Mail auf **Suchcode**.

   ![](assets/five-2.png)

1. Geben Sie ein, was Sie suchen möchten, und klicken Sie auf **Weitersuchen**, um vorwärts zu suchen, oder **Vorherige suchen**, um rückwärts zu suchen. Sie haben auch die Option **Ersetzen** und **Alle ersetzen**.

   ![](assets/six-1.png)

1. Klicken Sie abschließend **Schließen**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Der Such-Code ist auch im [E-Mail-Vorlageneditor](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md) verfügbar.

Es wird empfohlen, E-Mails weiterhin mit den integrierten Funktionen von Marketo zu bearbeiten. Dieser Code-Editor bietet jedoch bei Bedarf Flexibilität.
