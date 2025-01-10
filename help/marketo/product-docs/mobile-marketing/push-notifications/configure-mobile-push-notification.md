---
unique-page-id: 7512454
description: Mobile Push-Benachrichtigung konfigurieren - Marketo-Dokumente - Produktdokumentation
title: Mobile Push-Benachrichtigung konfigurieren
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 736e21d45d8a62e50f449e0ee6d0fc4df5963dfb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Mobile Push-Benachrichtigung konfigurieren {#configure-mobile-push-notification}

1. Navigieren Sie zum Bereich **Marketing** Aktivitäten.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Wählen Sie Ihr Push-Asset aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Navigieren Sie zu **Setup**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Wählen Sie Ihre gewünschte App aus. Android- und Apple-Plattformen sind standardmäßig aktiviert.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Wenn Ihre Push-Benachrichtigung nur für eine Plattform gilt (z. B. für iPhones), können Sie die andere Plattform ausschließen, indem Sie deren Selektor auf Deaktiviert verschieben.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Geben Sie den Nachrichtentext ein oder wählen Sie das Token-Symbol aus, um Token hinzuzufügen. Wählen Sie dann eine **Tipp-Aktion** aus.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Wenn eine Plattform aktiviert ist, wird sie auf der linken Seite des Telefonbildschirms angezeigt. Es wird farbig angezeigt, wenn es ausgewählt ist.

   >[!NOTE]
   >
   >Es gibt drei Arten von Tipp-Aktionen:
   >
   >**Launch App** - **Diese App** öffnet die Startseite Ihrer App, wenn auf die Benachrichtigung getippt wird. **Benutzerdefiniert** verwendet einen Deep-Link, um andere Bereiche Ihrer App oder einer anderen App zu öffnen, zu der Sie den Link haben (weitere Informationen finden [ unter Deep-Link-](#deep-link-uris)).
   >
   >**Landingpage** - Bringt Sie zu einer bestimmten Marketo-Landingpage.
   >
   >**Externe URL** - Bringt Sie zu einer Landingpage, die nicht zu Marketo gehört.

1. Um einen Deep-Link für eine benutzerdefinierte Tipp-Aktion einzufügen, klicken Sie auf Benutzerdefiniert und geben [Deep-Link-URI](#deep-link-uris) in das Feld ein.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Um Token einzufügen, wählen Sie ein Token aus, geben Sie einen Standardwert ein und klicken Sie auf „Einfügen“.

   >[!NOTE]
   >
   >Token werden an der Stelle angezeigt, an der Sie den Cursor in das Textfeld setzen. Sie können mehr als ein Token verwenden.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Nachrichten und Tipp-Aktionen sehen auf beiden Plattformen gleich aus.

1. Markieren Sie nur für iOS das Kontrollkästchen, um der App mitzuteilen, dass bei Eintreffen der Nachricht ein Ton abgespielt werden soll. Android spielt den Ton automatisch ab.

   ![](assets/ios-tap-and-notification-hand.png)

1. Zeigen Sie eine Vorschau der anderen Plattform an und klicken Sie auf **Beenden**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Klicken Sie **Genehmigen und schließen**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Herzlichen Glückwunsch! Jetzt kann die Push-Benachrichtigung gesendet werden.

## Deep-Link-URIs {#deep-link-uris}

Wenn Abonnentinnen und Abonnenten in einer Push-Nachricht auf eine Schaltfläche klicken, können sie entweder zur Startseite Ihrer App oder direkt zu einer bestimmten Seite innerhalb der App geleitet werden. Ein Deep-Link ist ein eindeutiger Verweis auf eine bestimmte Seite in Ihrer App und sieht einem Website-Link sehr ähnlich.

Ein Deep-Link-URI besteht aus drei Teilen: Schemaname, Pfad und Kennung. Im folgenden Beispiel ist „myappname“ das Schema. Der Pfad lautet „products“ und die Kennung lautet „purple-shirt“. Wenn der Kunde auf tippt, wird er speziell zum lilafarbenen Hemdenartikel auf den Produktseiten Ihrer App weitergeleitet.

![](assets/image2016-7-29-12-3a49-3a1.png)

Die Deep-Link-Struktur Ihrer App kann sich jedoch vom obigen Beispiel unterscheiden. Ihr Entwickler hat viele Optionen zum Definieren von Deep-Link-URIs. Bitten Sie Ihren Entwickler daher, Ihnen die URIs (Links) für die Seiten zu senden, die Sie verwenden möchten. Dadurch wird sichergestellt, dass die URIs, die Sie in Push-Nachrichten eingeben, an die richtigen Stellen zeigen. Ihr Entwickler kann [weitere Informationen finden Sie hier](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Mobile Push-Benachrichtigung senden](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
