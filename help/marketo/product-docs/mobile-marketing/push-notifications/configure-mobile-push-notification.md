---
unique-page-id: 7512454
description: Mobile Push-Benachrichtigung konfigurieren - Marketo-Dokumente - Produktdokumentation
title: Mobile Push-Benachrichtigung konfigurieren
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Mobile Push-Benachrichtigung konfigurieren {#configure-mobile-push-notification}

1. Navigieren Sie zu **Marketingaktivitäten** Bereich.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Wählen Sie Ihr Push-Asset aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Navigieren Sie zu **Einrichtung**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Wählen Sie die gewünschte App aus. Android- und Apple-Plattformen sind standardmäßig aktiviert.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Wenn Ihre Push-Nachricht nur für eine Plattform gilt (z. B. für iPhones), können Sie die andere Plattform ausschließen, indem Sie deren Auswahl auf Deaktiviert verschieben.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Klicks **Nächste**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Geben Sie den Nachrichtentext ein oder wählen Sie das Tokensymbol aus, um Token hinzuzufügen. Wählen Sie anschließend eine **Tippen Sie auf Aktion**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Wenn eine Plattform aktiviert ist, wird sie auf der linken Seite des Telefonbildschirms angezeigt. Er wird bei seiner Auswahl farbig angezeigt.

   >[!NOTE]
   >
   >Es gibt drei Arten von Tippen-Aktionen:
   >
   >**App starten** - **Diese App** öffnet die Startseite Ihrer App, wenn auf die Benachrichtigung getippt wird. **Benutzerdefiniert** verwendet einen Deep-Link, um andere Bereiche Ihrer App oder anderer Apps zu öffnen, zu denen Sie den Link haben (siehe [Deep-Link-URIs](#Deeplink) weiter unten).
   >
   >**Landingpage** - führt Sie zu einer bestimmten Marketo-Landingpage.
   >
   >**Externe URL** - führt Sie zu einer Landingpage, die nicht von Marketo stammt.

1. Um einen Deep-Link für eine benutzerdefinierte Tickaktion einzufügen, klicken Sie auf Benutzerdefiniert und geben Sie die [Deep-Link-URI](#Deeplink) im Feld.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Um Token einzufügen, wählen Sie ein Token aus, geben Sie einen Standardwert ein und klicken Sie auf &quot;Einfügen&quot;.

   >[!NOTE]
   >
   >Token werden dort angezeigt, wo Sie den Cursor in das Textfeld setzen. Sie können mehr als ein Token verwenden.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Nachrichten und Tippen-Aktionen sehen auf beiden Plattformen gleich aus.

1. Aktivieren Sie nur für iOS das Kontrollkästchen, damit die App beim Eintreffen der Nachricht einen Ton abspielen kann. Android gibt den Ton automatisch wieder.

   ![](assets/ios-tap-and-notification-hand.png)

1. Vorschau der anderen Plattform anzeigen und auf **Beenden**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Klicks **Genehmigen und schließen**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Herzlichen Glückwunsch! Jetzt kann die Push-Benachrichtigung gesendet werden.

## Deep-Link-URIs {#deep-link-uris}

Wenn Abonnenten auf eine Schaltfläche in einer Push-Nachricht klicken, gelangen sie entweder zur Startseite Ihrer App oder direkt zu einer bestimmten Seite in der App. Ein Deep-Link ist ein eindeutiger Verweis auf eine bestimmte Seite in Ihrer App und ähnelt sehr stark einem Website-Link.

Ein Deep-Link-URI besteht aus drei Teilen: Schemaname, Pfad und Kennung. Im folgenden Beispiel ist &quot;myappname&quot;das Schema. &quot;products&quot;ist der Pfad und &quot;lilafarbenes Shirt&quot;ist die Kennung. Wenn der Kunde tippt, werden diese speziell zum lilafarbenen Shirt-Element auf den Produktseiten Ihrer App geleitet.

![](assets/image2016-7-29-12-3a49-3a1.png)

Allerdings unterscheidet sich die Deep-Link-Struktur Ihrer App möglicherweise vom obigen Beispiel. Ihr Entwickler hat viele Möglichkeiten, Deep-Link-URIs zu definieren. Bitten Sie daher Ihren Entwickler, Ihnen die URIs (Links) für die Seiten zu senden, die Sie verwenden möchten. Dadurch wird sichergestellt, dass die in Push-Nachrichten eingegebenen URIs an die richtigen Stellen verweisen. Ihr Entwickler kann [Weitere Informationen finden Sie hier .](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Mobile Push-Benachrichtigung senden](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
