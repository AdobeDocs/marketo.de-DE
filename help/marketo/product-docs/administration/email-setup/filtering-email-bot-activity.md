---
description: Filtern der E-Mail-Bot-Aktivität - Marketo-Dokumente - Produktdokumentation
title: Filtern der E-Mail-Bot-Aktivität
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 32e635cf2c37f078737103653c706ad7b1afb515
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Filtern der E-Mail-Bot-Aktivität {#filtering-email-bot-activity}

Manchmal kann die E-Mail-Bot-Aktivität fälschlicherweise die Daten Ihrer E-Mail-Öffnungen und Klicks verfälschen. Führen Sie die folgenden Schritte aus, um dies zu beheben.

Wir verwenden drei verschiedene Methoden zur Bestätigung von Bot-Aktivitäten:

* Übereinstimmung mit [Bot-Liste des Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}: Aktivitäten, die mit irgendetwas in der Liste &quot;IAB UA/IP&quot;(Benutzeragent/IP-Adresse) übereinstimmen, werden als Bots markiert.
* Übereinstimmung mit dem Annäherungsmuster: Wenn mehrere Aktivitäten gleichzeitig stattfinden (in einer Sekunde), werden sie als Bots identifiziert.

Bei der Aktivität E-Mail-Link-Klick und E-Mail-Öffnung werden neue Attribute mit den folgenden Werten ausgefüllt:

* Aktivitäten, die als Bots identifiziert werden, haben &quot;Bot Activity&quot;als &quot;True&quot;und &quot;Bot Activity Pattern&quot;als identifiziertes Muster/Methode
* Aktivitäten, die als nicht &quot;bots&quot;gekennzeichnet sind, haben &quot;Bot Activity&quot;als &quot;False&quot;und &quot;Bot Activity Pattern&quot;als &quot;K/A&quot;.
* Aktivitäten, die stattgefunden haben, bevor wir diese Attribute eingeführt haben, haben &quot;Bot Activity&quot;als &quot;&quot;(leer) und &quot;Bot Activity Pattern&quot;als &quot;&quot;(leer).

1. Klicken **Admin**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicken **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicken Sie auf **Bot-Aktivität** Registerkarte.

   ![](assets/filtering-email-bot-activity-3.png)

1. Wählen Sie **Übereinstimmung mit IAB-Liste**, **Übereinstimmung mit Näherungsmuster** oder beides. Auswählen, ob eine Bot-Aktivität protokolliert werden soll _oder_ Filtern von Bot-Aktivitäten.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Wenn Sie &quot;Bot-Aktivität filtern&quot;auswählen, wird möglicherweise ein Rückgang bei E-Mail-Öffnungen und Klicks angezeigt, da falsche Aktivitäten ausgeschaltet werden.

**OPTIONALER SCHRITT**: Um diese Funktion zu deaktivieren, deaktivieren Sie einfach die Schieberegler. Wenn Sie deaktivieren, werden die Daten nicht zurückgesetzt.

>[!TIP]
>
>Nutzen Sie Bot-Aktivitätsdaten in Smart-Listen über die booleschen Werte &quot;Is Bot Activity&quot;(Ja/Nein) und &quot;Bot Activity Pattern&quot;in den Filtern &quot;Clicked Link in Email&quot;und &quot;Open Email&quot;, sowie &quot;Clicks Link in Email&quot;und &quot;Opens Email&quot;.
