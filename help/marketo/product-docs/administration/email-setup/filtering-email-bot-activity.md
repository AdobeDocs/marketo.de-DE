---
description: Filtern der E-Mail-Bot-Aktivität - Marketo-Dokumente - Produktdokumentation
title: Bot-Aktivität für E-Mails filtern
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: f3d0b2be794ca4bb6c38c942cef1fa72fe091d7c
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Bot-Aktivität für E-Mails filtern {#filtering-email-bot-activity}

Manchmal kann die E-Mail-Bot-Aktivität fälschlicherweise die Daten Ihrer E-Mail-Öffnungen und Klicks aufblähen. Gehen Sie wie folgt vor, um dieses Problem zu beheben.

Wir verwenden zwei verschiedene Methoden zum Bestätigen der Bot-Aktivität:

* Übereinstimmung mit der [Interactive Advertising Bureau Bot List](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: Aktivitäten, die mit irgendetwas auf der IAB UA/IP (User Agent/IP Address)-Liste übereinstimmen, werden als Bots markiert.
* Übereinstimmung mit dem Übereinstimmungsmuster: Wenn zwei oder mehr Aktivitäten gleichzeitig stattfinden (in weniger als einer Sekunde), werden sie als Bots identifiziert. Beim Vergleich werden folgende Attribute berücksichtigt:
   * Lead-ID (muss gleich sein)
   * E-Mail-Asset (muss dasselbe sein)
   * Link-Klick oder E-Mail öffnen
   * Zeitdifferenz (sollte weniger als eine Sekunde betragen)

Für die Aktivität E-Mail-Link-Klick und E-Mail-Öffnen werden neue Attribute mit den folgenden Werten ausgefüllt:

* Aktivitäten, die als Bots identifiziert werden, haben „Bot-Aktivität“ als „True“ und „Bot-Aktivitätsmuster“ als identifiziertes Muster/Methode
* Aktivitäten, die als nicht Bots identifiziert werden, haben „Bot Activity“ als „False“ und „Bot Activity Pattern“ als „N/A“
* Aktivitäten, die vor der Einführung dieser Attribute stattfanden, haben „Bot-Aktivität“ als &quot;&quot; (leer) und „Bot-Aktivitätsmuster“ als &quot;&quot; (leer)

## Filtertyp auswählen {#select-filter-type}

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Bot-Aktivität“.

   ![](assets/filtering-email-bot-activity-3.png)

1. Es stehen zwei Schieberegler zur Auswahl. Sie können nur ein oder beide aktivieren. Wenn Sie &quot;**[!UICONTROL mit IAB-Liste abgleichen]** aktivieren, wählen Sie aus, ob [!UICONTROL Bot-Aktivität &#x200B;] _oder_ [!UICONTROL Bot-Aktivität filtern].

   ![](assets/filtering-email-bot-activity-4.png)

1. Wenn Sie &quot;**[!UICONTROL mit Übereinstimmungsmuster“ aktivieren]** wählen Sie aus, ob [!UICONTROL Bot-Aktivität protokollieren] _oder_ [!UICONTROL Bot-Aktivität filtern]. Sie können auch die Anzahl der Sekunden für **Dauer zwischen Aktivitäten** festlegen (Standard ist 0, max ist 3).

   ![](assets/filtering-email-bot-activity-5.png)

>[!NOTE]
>
>Wenn **Dauer zwischen Aktivitäten** auf 0 Sekunden eingestellt ist, identifizieren wir E-Mail-Aktivitäten, die genau in der gleichen Sekunde stattfinden. Wenn innerhalb der angegebenen Anzahl von Sekunden mehrere E-Mail-Aktivitäten auftreten, wird sie als Bot-Aktivität identifiziert.

>[!IMPORTANT]
>
>* Wenn Sie [!UICONTROL Bot-Aktivität filtern] auswählen, werden möglicherweise weniger E-Mail-Öffnungen und Klicks angezeigt, da falsche Aktivitäten entfernt werden.

**OPTIONALER SCHRITT**: Um eine dieser Funktionen zu deaktivieren, heben Sie einfach die Auswahl des entsprechenden Schiebereglers auf. Andernfalls werden die Daten nicht zurückgesetzt.

>[!TIP]
>
>Nutzen Sie Bot-Aktivitätsdaten in Smart Lists über den booleschen Wert „Ist Bot-Aktivität“ (ja/nein) und das „Bot-Aktivitätsmuster“ in den Filtern „Klickter Link in E-Mail“ und „E-Mail öffnen“ sowie die Trigger „Klicks auf Link in E-Mail“ und „Öffnet E-Mail“.

## IP-Blockierungsliste {#ip-blocklist}

Wir haben eine Liste von IP-Adressen zusammengestellt, die für die Generierung von Millionen von gefälschten Interaktionen verantwortlich sind, da solche Interaktionen, die von einer der folgenden IPs empfangen werden, automatisch herausgefiltert und nicht zu Ihrer Marketo Engage-Instanz hinzugefügt werden. Dies kann zu einer Verringerung der E-Mail-Öffnungen, Klicks und anderer damit verbundener Aktivitäten führen. Die nachstehende Liste kann regelmäßig aktualisiert werden.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54.71.187.124
* 60.28.2.248
* 64.235.150.252
* 64.235.153.10
* 64.235.153.2
* 64.235.154.105
* 64.235.154.109
* 64.235.154.140
* 64.74.215.1
* 64.74.215.100
* 64.74.215.138
* 64.74.215.139
* 64.74.215.142
* 64.74.215.146
* 64.74.215.150
* 64.74.215.154
* 64.74.215.158
* 64.74.215.162
* 64.74.215.164
* 64.74.215.166
* 64.74.215.170
* 64.74.215.174
* 64.74.215.176
* 64.74.215.178
* 64.74.215.51
* 64.74.215.56
* 64.74.215.58
* 64.74.215.59
* 64.74.215.86
* 64.74.215.98
* 65.154.226.101
* 66.249.91.149
* 70.42.131.106
* 74.125.217.116
* 74.217.90.250
* 104.129.41.4
* 104.47.55.126
* 104.47.58.126
* 104.47.70.126
* 104.47.73.126
* 104.47.73.254
* 104.47.74.126
* 128.220.160.1
* 155.70.39.101
* 162.129.251.14
* 162.129.251.42
* 208.52.157.204

>[!NOTE]
>
>Wir analysieren und prüfen jede IP-Adresse sorgfältig, bevor wir sie dieser Liste hinzufügen, um sicherzustellen, dass nur die kritischsten und schädlichsten IP-Adressen blockiert werden.
