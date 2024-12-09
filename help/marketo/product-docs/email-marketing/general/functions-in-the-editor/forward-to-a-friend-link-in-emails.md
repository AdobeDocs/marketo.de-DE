---
unique-page-id: 1900581
description: Weiterleiten an einen Freunde-Link in E-Mails - Marketo-Dokumente - Produktdokumentation
title: Weiterleiten an einen Freunde-Link in E-Mails
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Weiterleiten an einen Freunde-Link in E-Mails {#forward-to-a-friend-link-in-emails}

Wenn Sie den Link &quot;Weiterleiten an Freunde&quot; zu Ihren E-Mails hinzufügen, können Sie Personen, die über diesen Link eine weitergeleitete E-Mail erhalten haben, verfolgen und diese automatisch als neue Person hinzufügen, wenn sie noch nicht in der Datenbank sind.

Angenommen, Keith verwendet den Link &quot;Weiterleiten an Freunde&quot;, um die E-Mail an eine unbekannte Person, Mark, weiterzuleiten. Mark wird automatisch als neue Person hinzugefügt, erhält sein eigenes Cookie und jede seiner E-Mail- und Web-Aktivitäten ist mit ihm verknüpft. Wenn Keith jedoch die Weiterleitungs-Schaltfläche in seinem E-Mail-Client verwendet, wird Mark fälschlicherweise als Keith-Cookie gesetzt und seine Aktivität wird als Keith&#39;s protokolliert.

## Link zu einer E-Mail-Vorlage hinzufügen {#add-the-link-to-an-email-template}

1. Wechseln Sie zu **Design Studio**.

   ![](assets/one-8.png)

1. Wählen Sie die E-Mail-Vorlage aus, zu der Sie den Link hinzufügen möchten. Klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/two-7.png)

1. Fügen Sie den folgenden HTML-Code an die Stelle ein, an der der Link &quot;Weiterleiten an Freunde&quot;angezeigt werden soll (wenn Sie Hilfe zu diesem Teil benötigen, wenden Sie sich bitte an Ihren Web-Entwickler):

   `<a href="{{system.forwardToFriendLink}}">Forward to Friend</a>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Sie können dem Link Stile hinzufügen, damit er schöner aussieht. Beispiel:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Es wird nicht empfohlen, den Stil **position:relative** in Ihrer E-Mail-Vorlage zu verwenden. Es können Probleme mit der Position und Anzeige des Felds &quot;Weiterleiten an Freunde&quot;auftreten.

1. Klicken Sie auf **Vorschau des Entwurfs anzeigen** , um sicherzustellen, dass die Vorlage wie gewünscht aussieht.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Denken Sie daran, den Vorlagenentwurf zu validieren, um die Änderungen anzuwenden.

   Jetzt haben alle E-Mails, die diese Vorlage verwenden, den Link &quot;Weiterleiten an Freunde&quot;. Wenn der E-Mail-Empfänger darauf klickt, wird er mit der Box &quot;Weiterleiten an einen Freund&quot;zu einer Web-Version der E-Mail weitergeleitet:

   ![](assets/f2afbox.png)

## Link zu einer einzelnen E-Mail hinzufügen {#add-the-link-to-an-individual-email}

Sie können den Link &quot;Weiterleiten an Freunde&quot;auch direkt in eine E-Mail einfügen.

1. Öffnen Sie die E-Mail, in der Sie den Link einfügen möchten, und doppelklicken Sie auf den bearbeitbaren Bereich.

   ![](assets/five-4.png)

1. Platzieren Sie den Cursor an die Stelle, an der der Link erscheinen soll, und klicken Sie auf die Schaltfläche **Token einfügen** .

   ![](assets/six-2.png)

1. Wählen Sie das **`{{system.forwardToFriendLink}}`** -Token aus.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Dieses Token ist die URL der Webversion der E-Mail mit dem Feld &quot;Weiterleiten an Freunde&quot;.

1. Schreiben Sie, was der Anzeigetext des Links sein soll (z. B. &quot;Weiterleiten an einen Freund&quot;).

   ![](assets/seven-1.png)

1. Ausschneiden des **`{{system.forwardToFriendLink}}`**-Tokens mit Strg+X (Windows) oder Befehl+X (Mac). Markieren Sie &quot;Weiterleiten an einen Freund&quot;und klicken Sie auf die Schaltfläche **Link einfügen/bearbeiten** .

   ![](assets/eight-1.png)

1. Fügen Sie das Token **`{{system.forwardToFriendLink}}`** mithilfe von Strg/Befehl+V in das Feld **URL** ein und klicken Sie dann auf **Einfügen**.

   ![](assets/nine.png)

1. Speichern Sie die Bearbeitung und sehen Sie sich Ihren neuen Link in der Vorschau an!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Neue Personen, die durch den Erhalt der E-Mail &quot;Weiterleiten an Freunde&quot;hinzugefügt werden, werden standardmäßig von Marketing-E-Mails abgemeldet.

## Weiterleitungsaktivität anzeigen {#view-forwarding-activity}

Sie können im Aktivitätsprotokoll der Person sehen, wer die E-Mails weitergeleitet und empfangen hat.

1. Wechseln Sie zu &quot;**`Database`**&quot;.

   ![](assets/db.png)

1. Doppelklicken Sie auf die Person, für die Sie die Aktivität anzeigen möchten.

   ![](assets/fourteen.png)

1. Gehen Sie zur Registerkarte **Aktivitätsprotokoll** . Doppelklicken Sie auf **Weitergeleitet an Freunde-E-Mail** oder auf **Weitergeleitet an Freunde-E-Mail** , um Details anzuzeigen.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >Für &quot;Weitergeleitet an Freunde-E-Mail&quot;ist die Personen-ID die Person, die die E-Mail weitergeleitet hat.
   >
   >Für &quot;Weitergeleitet an Freunde-E-Mail&quot;ist die Personen-ID die Person, die die E-Mail erhalten hat.

   ![](assets/sixteen.png)

1. Um eine Person nach ID anzuzeigen, kopieren Sie die **Personen-ID** und fügen Sie sie am Ende der URL ein (der Anfang der URL hängt von Ihrer Marketo-Instanz ab):

   `...marketo.com/Database/loadPersonDetail?personId=`

   >[!NOTE]
   >
   >Wir machen die **Personen-ID** anklickbar und verknüpfen sie direkt mit der Person in einem kommenden Patch.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Wenn der Freund, der den Vorwärts erhält, eine unbekannte Person ist, wird eine neue Person mit &quot;Weiterleiten an Freunde&quot;erstellt, die als **Source** der Person markiert ist.
   >Wenn die E-Mail ein lokales Asset eines Programms ist, wird das Programm als **Akquiseprogramm** der Person markiert.

## Trigger oder Filter mit der Aktivität &quot;Weiterleitung&quot; {#trigger-or-filter-using-forwarding-activity}

Es gibt sechs Trigger/Filter, mit denen Sie Aktionen zum Trigger von Datenflüssen durchführen oder Personen nach gesendeter und empfangener Aktivität &quot;Weiterleiten an Freunde&quot;filtern können.

Wenn Sie in der Smart-Liste einer Smart-Kampagne nach &quot;forward&quot;suchen, finden Sie die verfügbaren Trigger und Filter.

![](assets/nineteen.png)

## Weiterleiten an Freunde testen {#test-forward-to-friend}

Um &quot;Weiterleiten an Freunde&quot;zu testen, senden Sie sich eine E-Mail mit dem Weiterleitungslink. Vergewissern Sie sich, dass Sie es über den Fluss **E-Mail senden** senden, *nicht* bis **Test-E-Mail senden**.
