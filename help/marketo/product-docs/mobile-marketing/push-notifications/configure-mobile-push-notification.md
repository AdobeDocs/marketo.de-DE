---
unique-page-id: 7512454
description: Mobile Push-Benachrichtigung konfigurieren - MarketingToDocs - Produktdokumentation
title: Mobile Push-Benachrichtigung konfigurieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Mobile Push-Benachrichtigung konfigurieren {#configure-mobile-push-notification}

1. Gehen Sie zum Bereich Marketing-Aktivitäten.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Wählen Sie Ihr Push-Asset aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Gehen Sie zu **Setup**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Wählen Sie die gewünschte App aus. Android- und Apple-Plattformen sind standardmäßig aktiviert.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   Wenn Ihre Push-Nachricht nur für eine Plattform gilt (z. B. für iPhones), können Sie die andere Plattform ausschließen, indem Sie ihre Auswahl auf Deaktiviert verschieben.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   Klicken Sie auf WEITER.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Geben Sie den Nachrichtentext ein oder wählen Sie das Tokensymbol aus, um Token hinzuzufügen. Wählen Sie dann eine **Aktion**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Wenn eine Plattform aktiviert ist, wird sie auf der linken Seite des Bildschirms angezeigt. Er wird bei Auswahl farbig angezeigt.

   >[!NOTE]
   >
   >**Definition**
   >
   >
   >Es gibt drei Arten von**-Tap-Aktionen:**
   >
   >
   >**App**  starten:  **Dieses** Apps öffnet die Startseite Ihrer App, wenn auf die Benachrichtigung getippt wird. **** Benutzerdefiniert öffnet einen Deep Link, um andere Bereiche Ihrer App oder einer anderen App zu öffnen, zu der Sie den Link haben (weitere Informationen finden Sie unter  [Deep Link-](#Deeplink) URIss unten).
   >
   >
   >**Landingpage**  - bringt Sie zu einer bestimmten Marketo-Landingpage.
   >
   >
   >**Externe URL**  - führt Sie zu einer Nicht-Marketo-Landingpage.

   Um einen Deep Link für eine benutzerdefinierte Tickaktion einzufügen, klicken Sie auf &quot;Benutzerdefiniert&quot;und geben Sie den [Deep-Link-URI](#Deeplink) in das Feld ein.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   Um Token einzufügen, wählen Sie ein Token aus, geben Sie einen Standardwert ein und klicken Sie auf Einfügen.

   >[!NOTE]
   >
   >Token werden an der Stelle angezeigt, an der Sie den Cursor in das Textfeld setzen. Sie können mehrere Token verwenden.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Nachrichten und Tippen-Aktionen sehen auf beiden Plattformen gleich aus.

   Markieren Sie das Kontrollkästchen nur für iOS, um der App mitzuteilen, dass sie beim Eintreffen der Nachricht einen Ton abspielen soll. Android gibt den Sound automatisch wieder.

   ![](assets/ios-tap-and-notification-hand.png)

   Vorschau der anderen Plattform und klicken Sie auf FINISH.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Klicken Sie auf **GENEHMIGEN UND SCHLIESSEN**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Herzlichen Glückwunsch! Die Push-Benachrichtigung kann jetzt gesendet werden.

## Deep-Link-URIs {#deep-link-uris}

Wenn Abonnenten auf eine Schaltfläche in einer Push-Nachricht klicken, können sie diese entweder zur Startseite Ihrer App oder direkt zu einer bestimmten Seite in der App führen. Ein Deep Link ist ein eindeutiger Verweis auf eine bestimmte Seite in Ihrer App und sieht sehr ähnlich aus wie ein Website-Link.

Ein Deep-Link-URI besteht aus drei Teilen: Schemaname, Pfad und ID. Im Beispiel unten ist &quot;myappname&quot;das Schema. &quot;products&quot;ist der Pfad, und &quot;purpurpurfarbenes Shirt&quot;ist der Bezeichner. Wenn der Kunde auf die App tippt, werden diese speziell zum violetten Hemdelement innerhalb der Produktseiten Ihrer App geleitet.

![](assets/image2016-7-29-12-3a49-3a1.png)

Allerdings kann sich die Deep-Link-Struktur Ihrer App vom oben genannten Beispiel unterscheiden. Ihr Entwickler hat viele Optionen zum Definieren von Deep-Link-URIs. Bitten Sie daher Ihren Entwickler, Ihnen die URIs (Links) für die Seiten zu senden, die Sie verwenden möchten. Dadurch wird sichergestellt, dass die URIs, die Sie in Push-Nachrichten eingeben, an die richtigen Stellen zeigen. Ihr Entwickler kann [hier weitere Informationen finden.](http://developers.marketo.com/mobile/enabling-deep-links-in-your-app/)

>[!MORELIKETHIS]
>
>* [Push-Benachrichtigung für Mobilgeräte senden](send-a-mobile-push-notification.md)

>



