---
unique-page-id: 13796466
description: Erste Schritte mit Sales Connect - Marketing Docs - Produktdokumentation
title: Erste Schritte mit Sales Connect
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---


# Erste Schritte mit Sales Connect {#getting-started-with-sales-connect}

Wenn Sie diese Schritte lieber ansehen als lesen möchten, gehen Sie direkt zu den [Videoanweisungen weiter unten](#video).

>[!NOTE]
>
>**Verfügbarkeit**
>
>Nicht alle Kunden haben diese Funktion erworben. Wenden Sie sich für weitere Informationen an Ihren Kundenbetreuer.

## Erste Schritte {#what-you-need-to-get-started}

* Marketo-Abonnement
* Sales Connect-Abonnement
* Salesforce-Abonnement (mit aktivierten API-Aufrufen und Apex-Klassen)

## Wen Sie beginnen müssen {#who-you-need-to-get-started}

* Marketing-Administrator-Benutzer
* Sales Connect-Admin-Benutzer
* Salesforce Admin
* Sales Connect-Benutzer

## Sales Connect-Administratoren {#sales-connect-admins}

Sie erhalten eine E-Mail von Marketo mit einem Link zum Zurücksetzen Ihres Kennworts. Nachdem Sie ein neues Kennwort erstellt haben, melden Sie sich bei Sales Connect an.

Um die Einrichtung abzuschließen, müssen Sie folgende Schritte ausführen:

* [Connect Sales Connect und Salesforce](#sfdc)
* [Anmeldeinformationen vor der Verbindung von Sales Connect mit Marketing abrufen](#acquire)
* [Verbindung von Verkaufsstellen mit Marketo](#mkto)
* [Benutzer einladen/bereitstellen](#IPU)

Optional können Sie auch:

* [Test Sales Connect in Ihrer Sandbox](#sandbox)

## Verbinden Sie Ihr Sales Connect-Konto mit Salesforce. {#connect-your-sales-connect-account-to-salesforce}

Gehen Sie wie in [diesem Artikel beschrieben vor, um Ihr Sales Connect-Konto als Administrator oder Nicht-Administrator mit Ihrem Salesforce-Konto zu verbinden](http://docs.marketo.com/x/JwDb).

>[!NOTE]
>
>Die Salesforce-Instanz, zu der Sie eine Verbindung herstellen, muss dieselbe Instanz sein, die mit Marketo verbunden ist (oder sein wird).

## Berechtigungen vor dem Herstellen einer Verbindung zwischen Vertrieb und Marketing abrufen {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Sie benötigen einen Satz Anmeldeinformationen aus Marketo. Diese Anmeldeinformationen werden später vom Sales Connect-Administrator verwendet, um Marketing mit Sales Connect zu verbinden.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie in der Struktur auf **Sales Connect**.

   ![](assets/two.png)

1. Wählen Sie die folgenden Marketing-Anmeldeinformationen aus und senden Sie sie an Ihren Sales Connect-Administrator: Munchkin-ID, Client-ID, geheimer Clientschlüssel.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Wenn Sie die oben genannten Informationen kopieren und einfügen, stellen Sie sicher, dass keine Leerzeichen hinzugefügt werden.

## Verbindung von Verkaufsstellen mit Marketing {#connect-sales-connect-to-marketo}

1. Klicken Sie in Sales Connect auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/four.png)

1. Wählen Sie unter &quot;Admin-Einstellungen&quot; **Markieren**.

   ![](assets/eight.png)

1. Geben Sie die vom Marketing-Administrator angegebenen Anmeldeinformationen ein und klicken Sie auf **Verbinden**.

   ![](assets/credentials.png)

## Benutzer einladen/bereitstellen {#invite-provision-users}

Wenn bereits Benutzer in Ihrem Konto vorhanden sind (zuvor von ToutApp), werden sie auf der Registerkarte &quot; **Teamzugriff** &quot;im Abschnitt &quot;Marketing&quot;von Sales Connect angezeigt.

Sie können Ihr Team als Marketing Connect-Benutzer auf dieser Seite bereitstellen. Wenn Sie ToutApp noch nie verwendet haben oder noch Benutzer einladen müssen, führen Sie die Schritte in [diesem Artikel](http://docs.marketo.com/display/TOUT/Invite+Team+Members)aus.

>[!CAUTION]
>
>Bitte warten Sie zehn Minuten nach der Verbindung von Sales Connect mit Marketo, bevor Sie diese Schritte durchführen.

1. Wählen Sie einen oder mehrere Benutzer aus und klicken Sie dann auf **Verbinden**.

   >[!NOTE]
   >
   >Sie können die Workspace-Zuweisung nur einmal ausführen, wenn Sie Benutzer einladen. Nach der Einstellung müssen Sie die Verbindung zum Benutzer trennen, um sie zu ändern.

   ![](assets/users.png)

1. Wenn für Ihr MarketingTo-Abonnement Arbeitsbereiche aktiviert sind, können Sie jedem Benutzer oder Benutzergruppen Arbeitsflächen zuweisen. Wenn keine Arbeitsbereiche ausgewählt sind, weisen wir sie dem Arbeitsbereich &quot;Standardmarkierung&quot;zu.

   ![](assets/nine.jpg)

1. Klicken Sie auf die Dropdownliste Arbeitsbereich, wählen Sie die gewünschten Arbeitsbereiche aus und klicken Sie auf **Verbinden**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Wenn Sie neue Benutzer hinzufügen möchten, wechseln Sie zum Abschnitt &quot;Teamverwaltung&quot;in den Admin-Einstellungen und klicken Sie auf die Schaltfläche &quot;Benutzer **einladen** &quot;.

Sie können weitere Benutzer über die Seite &quot;Teamverwaltung&quot;aufrufen und die oben beschriebenen Schritte ausführen, um eine Verbindung herzustellen.

## Test Sales Connect in Ihrer Sandbox {#test-sales-connect-in-your-sandbox}

Für Teams, die Marketo Sales Connect mit ihrer Marketo Sandbox testen möchten, kann auf Anfrage ein zusätzliches Sales Connect-Konto bereitgestellt werden. Dies gilt nur für Kunden, die eine Marketo Sandbox gekauft haben, oder für Kunden, die diese als Teil ihres Marketo-Bundles haben. Wenn Sie eine Sandbox erwerben möchten, wenden Sie sich bitte an Ihren Marketing-Kundenbetreuer.

>[!NOTE]
>
>Sie können für mehrere Instanzen kein Sales Connect-Konto mit derselben E-Mail-ID bereitstellen. Wenn Sie also ein zusätzliches Sales Connect-Konto zum Testen mit Ihrer Marketing Sandbox-Instanz haben möchten, müssen Sie in jedem Konto eine andere E-Mail-ID verwenden.

## Videoanweisungen {#video-instructions}

`<iframe width="630" height="470" src="//play.vidyard.com/w5RY7iMPpEfUYQ4Fp8WUKR.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`
