---
unique-page-id: 13796466
description: Erste Schritte mit Sales Connect - Marketo Docs - Produktdokumentation
title: Erste Schritte mit Sales Connect
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Erste Schritte mit Sales Connect {#getting-started-with-sales-connect}

Wenn Sie diese Schritte lieber als gelesen ansehen möchten, gehen Sie direkt zu den [Videoanweisungen unter](#video).

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Wenden Sie sich für weitere Informationen an Ihren Kundenbetreuer.

## Was Sie zum Einstieg benötigen{#what-you-need-to-get-started}

* Marketo Abonnement
* Sales Connect-Abonnement
* Salesforce-Abonnement (mit aktivierten API-Aufrufen und Apex-Klassen)

## Wen Sie anfangen müssen {#who-you-need-to-get-started}

* Marketo Admin-Benutzer
* Sales Connect-Admin-Benutzer
* Salesforce Admin
* Sales Connect-Benutzer

## Sales Connect-Administratoren {#sales-connect-admins}

Sie erhalten eine E-Mail von Marketo mit einem Link zum Zurücksetzen Ihres Kennworts. Nachdem Sie ein neues Kennwort erstellt haben, melden Sie sich bei Sales Connect an.

Um die Einrichtung abzuschließen, müssen Sie folgende Schritte ausführen:

* [Connect Sales Connect und Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [Anmeldeinformationen vor der Verbindung von Sales Connect mit Marketo erwerben](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connect Sales Connect mit Marketo](#connect-sales-connect-to-marketo)
* [Benutzer einladen/bereitstellen](#invite-provision-users)

Optional können Sie auch:

* [Test Sales Connect in Ihrer Sandbox](#test-sales-connect-in-your-sandbox)

## Verbinden Sie Ihr Sales Connect-Konto mit Salesforce {#connect-your-sales-connect-account-to-salesforce}

Um Ihr Sales Connect-Konto mit Ihrem Salesforce-Konto als Administrator oder Nicht-Administrator zu verbinden, führen Sie die Schritte unter [diesen Artikel](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md) aus.

>[!NOTE]
>
>Die Salesforce-Instanz, zu der Sie eine Verbindung herstellen, muss dieselbe Instanz sein, die mit Marketo verbunden ist (oder sein wird).

## Berechtigungen vor der Verbindung von Vertrieb mit Marketo abrufen {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Sie benötigen einen Satz Anmeldeinformationen aus Marketo. Diese Anmeldeinformationen werden später vom Sales Connect-Administrator verwendet, um Marketo mit Sales Connect zu verbinden.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie in der Struktur auf **Verkaufsverbindung**.

   ![](assets/two.png)

1. Wählen Sie die folgenden Marketo-Anmeldedaten aus und senden Sie sie an Ihren Sales Connect-Administrator: Munchkin-ID, Client-ID, geheimer Clientschlüssel.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Wenn Sie die oben genannten Informationen kopieren und einfügen, stellen Sie sicher, dass keine Leerzeichen hinzugefügt werden.

## Connect Sales Connect mit Marketo {#connect-sales-connect-to-marketo}

1. Klicken Sie in Sales Connect auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/four.png)

1. Wählen Sie unter &quot;Admin-Einstellungen&quot;die Option **Marketo**.

   ![](assets/eight.png)

1. Geben Sie die vom Marketo-Administrator angegebenen Marketo-Anmeldeinformationen ein und klicken Sie auf **Connect**.

   ![](assets/credentials.png)

## Benutzer einladen/bereitstellen {#invite-provision-users}

Wenn bereits Benutzer in Ihrem Konto vorhanden sind (zuvor von ToutApp), werden sie auf der Registerkarte **Teamzugriff** im Marketo-Abschnitt von Sales Connect angezeigt.

Auf dieser Seite können Sie Ihr Team als Marketo Sales Connect-Benutzer bereitstellen. Wenn Sie ToutApp noch nie verwendet haben oder noch Benutzer einladen müssen, befolgen Sie die Schritte in [diesem Artikel](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md).

>[!CAUTION]
>
>Bitte warten Sie zehn Minuten nach der Verbindung von Sales Connect mit Marketo, bevor Sie diese Schritte durchführen.

1. Wählen Sie einen oder mehrere Benutzer aus und klicken Sie dann auf **Verbinden**.

   >[!NOTE]
   >
   >Sie können die Workspace-Zuweisung nur einmal ausführen, wenn Sie Benutzer einladen. Nach der Einstellung müssen Sie die Verbindung zum Benutzer trennen, um sie zu ändern.

   ![](assets/users.png)

1. Wenn Ihr Marketo-Abonnement Arbeitsbereiche aktiviert hat, können Sie jedem Benutzer oder Benutzergruppen Arbeitsflächen zuweisen. Wenn keine Arbeitsbereiche ausgewählt sind, weisen wir sie dem Standard-Arbeitsbereich von Marketo zu.

   ![](assets/nine.jpg)

1. Klicken Sie auf die Dropdownliste Arbeitsbereich, wählen Sie die gewünschten Arbeitsbereiche aus und klicken Sie auf **Verbinden**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Wenn Sie neue Benutzer hinzufügen möchten, wechseln Sie zum Abschnitt &quot;Teamverwaltung&quot;in den Admin-Einstellungen und klicken Sie auf die Schaltfläche **Benutzer einladen**.

Sie können weitere Benutzer über die Seite &quot;Teamverwaltung&quot;aufrufen und die oben beschriebenen Schritte ausführen, um eine Verbindung herzustellen.

## Test Sales Connect in Ihrer Sandbox {#test-sales-connect-in-your-sandbox}

Für Teams, die Marketo Sales Connect mit ihrer Marketo Sandbox testen möchten, kann auf Anfrage ein zusätzliches Sales Connect-Konto eingerichtet werden. Dies gilt nur für Kunden, die eine Marketo Sandbox gekauft haben, oder für Kunden, die diese im Rahmen ihres Marketo Bundles erworben haben. Wenn Sie eine Sandbox erwerben möchten, wenden Sie sich bitte an Ihren Marketo Kundenbetreuer.

>[!NOTE]
>
>Sie können für mehrere Instanzen kein Sales Connect-Konto mit derselben E-Mail-ID bereitstellen. Wenn Sie also ein zusätzliches Sales Connect-Konto zum Testen mit Ihrer Marketo Sandbox-Instanz haben möchten, müssen Sie in jedem Konto eine andere E-Mail-ID verwenden.
