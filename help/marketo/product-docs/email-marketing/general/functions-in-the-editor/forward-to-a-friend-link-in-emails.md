---
unique-page-id: 1900581
description: Weiterleiten an einen Freunde-Link in E-Mails - Marketo-Dokumente - Produktdokumentation
title: Weiterleiten an einen Freunde-Link in E-Mails
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Weiterleiten an einen Freunde-Link in E-Mails {#forward-to-a-friend-link-in-emails}

Wenn Sie den Link &quot;Weiterleiten an Freunde&quot;zu Ihren E-Mails hinzufügen, können Sie Personen, die über diesen Link eine weitergeleitete E-Mail erhalten haben, verfolgen und sie automatisch als neue Person hinzufügen, wenn sie noch nicht in der Datenbank sind.

Angenommen, Keith verwendet den Link &quot;Weiterleiten an Freunde&quot;, um die E-Mail an eine unbekannte Person, Mark, weiterzuleiten. Mark wird automatisch als neue Person hinzugefügt, erhält sein eigenes Cookie und jede seiner E-Mail- und Web-Aktivitäten ist mit ihm verknüpft. Wenn Keith jedoch die Weiterleitungs-Schaltfläche in seinem E-Mail-Client verwendet, wird Mark fälschlicherweise als Keith-Cookie gesetzt und seine Aktivität wird als Keith&#39;s protokolliert.

## Link zu einer E-Mail-Vorlage hinzufügen {#add-the-link-to-an-email-template}

1. Navigieren Sie zu **Design Studio**.

   ![](assets/one-8.png)

1. Wählen Sie die E-Mail-Vorlage aus, zu der Sie den Link hinzufügen möchten. Klicken **Entwurf bearbeiten**.

   ![](assets/two-7.png)

1. Fügen Sie den folgenden HTML-Code an die Stelle ein, an der der Link &quot;Weiterleiten an Freunde&quot;angezeigt werden soll (wenn Sie Hilfe zu diesem Teil benötigen, wenden Sie sich bitte an Ihren Web-Entwickler):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Sie können dem Link Stile hinzufügen, damit er schöner aussieht. Beispiel:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Es wird nicht empfohlen, die Formatierung zu verwenden **position:relative** in Ihrer E-Mail-Vorlage. Es kann zu Problemen mit der Position und Anzeige der Box &quot;Weiterleiten an Freunde&quot;führen.

1. Klicken **Vorschau des Entwurfs** , um sicherzustellen, dass die Vorlage wie gewünscht aussieht.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Denken Sie daran, den Vorlagenentwurf zu validieren, um die Änderungen anzuwenden.

   Jetzt haben alle E-Mails, die diese Vorlage verwenden, den Link &quot;Weiterleiten an Freunde&quot;. Wenn der E-Mail-Empfänger darauf klickt, wird er mit dem Feld &quot;Weiterleiten an einen Freund&quot;zu einer Web-Version der E-Mail weitergeleitet:

   ![](assets/f2afbox.png)

## Link zu einer einzelnen E-Mail hinzufügen {#add-the-link-to-an-individual-email}

Sie können den Link &quot;Weiterleiten an Freunde&quot;auch direkt in eine E-Mail einfügen.

1. Öffnen Sie die E-Mail, in der Sie den Link einfügen möchten, und doppelklicken Sie auf den bearbeitbaren Bereich.

   ![](assets/five-4.png)

1. Platzieren Sie den Cursor an die Stelle, an der der Link angezeigt werden soll, und klicken Sie auf **Token einfügen** Schaltfläche.

   ![](assets/six-2.png)

1. Wählen Sie die **`{{system.forwardToFriendLink}}`** Token.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Dieses Token ist die URL der Webversion der E-Mail mit dem Feld &quot;Weiterleiten an Freunde&quot;.

1. Schreiben Sie, was der Anzeigetext des Links sein soll (z. B. &quot;Weiterleiten an einen Freund&quot;).

   ![](assets/seven-1.png)

1. Ausschneiden der **`{{system.forwardToFriendLink}}`** Token mit Strg+X (Windows) oder Befehl+X (Mac). Markieren Sie &quot;Weiterleiten an einen Freund&quot;und klicken Sie auf die **Link einfügen/bearbeiten** Schaltfläche.

   ![](assets/eight-1.png)

1. Fügen Sie die **`{{system.forwardToFriendLink}}`** Token in **URL** Feld mit Strg/Befehl+V und klicken Sie dann auf **Einfügen**.

   ![](assets/nine.png)

1. Speichern Sie die Bearbeitung und sehen Sie sich Ihren neuen Link in der Vorschau an!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Neue Personen, die durch Erhalt der E-Mail &quot;Weiterleiten an Freunde&quot;hinzugefügt werden, werden standardmäßig von Marketing-E-Mails abgemeldet.

## Weiterleitungsaktivität anzeigen {#view-forwarding-activity}

Sie können im Aktivitätsprotokoll der Person sehen, wer die E-Mails weitergeleitet und empfangen hat.

1. Navigieren Sie zu **`Database`**.

   ![](assets/db.png)

1. Doppelklicken Sie auf die Person, für die Sie die Aktivität anzeigen möchten.

   ![](assets/fourteen.png)

1. Navigieren Sie zu **Aktivitätsprotokoll** Registerkarte. Doppelklicken **Weiterleiten an Freunde-E-Mail erhalten** oder **Weiterleiten an Freunde-E-Mail** um Details anzuzeigen.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >Für &quot;Weitergeleitet an Freunde-E-Mail&quot;ist die Personen-ID die Person, die die E-Mail weitergeleitet hat.
   >
   >Für &quot;Weitergeleitet an Freunde-E-Mail&quot;ist die Personen-ID die Person, die die E-Mail erhalten hat.

   ![](assets/sixteen.png)

1. Um eine Person nach ID anzuzeigen, kopieren Sie die **Personen-ID** an das Ende der URL (der Anfang dieser URL hängt von Ihrer Marketo-Instanz ab):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Wir werden **Personen-ID** anklickbar und verlinken Sie direkt mit der Person in einem anstehenden Patch.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Wenn der Freund, der den Weiterleiten erhält, eine unbekannte Person ist, wird eine neue Person mit der Bezeichnung &quot;Weiterleiten an Freunde&quot;als **Quelle**.
   >Wenn die E-Mail ein lokales Asset eines Programms ist, wird das Programm als **Akquiseprogramm**.

## Trigger oder Filter mit der Aktivität &quot;Weiterleitung&quot; {#trigger-or-filter-using-forwarding-activity}

Es gibt sechs Trigger/Filter, mit denen Sie Aktionen zum Trigger von Datenflüssen durchführen oder Personen nach gesendeter und empfangener Aktivität &quot;Weiterleiten an Freunde&quot;filtern können.

Wenn Sie in der Smart-Liste einer Smart-Kampagne nach &quot;forward&quot;suchen, finden Sie die verfügbaren Trigger und Filter.

![](assets/nineteen.png)

## Weiterleiten an Freunde testen {#test-forward-to-friend}

Um &quot;Weiterleiten an Freunde&quot;zu testen, senden Sie sich eine E-Mail mit dem Weiterleitungslink. Vergewissern Sie sich, dass der Versand über die **E-Mail senden** Flussschritt, *not* bis **Test-E-Mail senden**.
