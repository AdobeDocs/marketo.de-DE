---
description: Filtern der E-Mail-Bot-Aktivität - Marketo-Dokumente - Produktdokumentation
title: Filtern der E-Mail-Bot-Aktivität
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 14%

---

# Filtern der E-Mail-Bot-Aktivität {#filtering-email-bot-activity}

Manchmal kann die E-Mail-Bot-Aktivität fälschlicherweise die Daten Ihrer E-Mail-Öffnungen und Klicks verfälschen. Führen Sie die folgenden Schritte aus, um dies zu beheben.

Zur Bestätigung der Bot-Aktivität werden zwei verschiedene Methoden verwendet:

* Übereinstimmung mit [Bot-Liste des Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: Aktivitäten, die mit irgendetwas in der Liste &quot;IAB UA/IP&quot;(Benutzeragent/IP-Adresse) übereinstimmen, werden als Bots markiert.
* Übereinstimmung mit dem Annäherungsmuster: Wenn mehrere Aktivitäten gleichzeitig stattfinden (in einer Sekunde), werden sie als Bots identifiziert. Beim Vergleich berücksichtigte Attribute sind:
   * Lead-ID (sollte identisch sein)
   * E-Mail-Asset (sollte identisch sein)
   * Link-Klick oder E-Mail-Öffnung
   * Zeitdifferenz (sollte weniger als eine Sekunde betragen)

Bei der Aktivität E-Mail-Link-Klick und E-Mail-Öffnung werden neue Attribute mit den folgenden Werten ausgefüllt:

* Aktivitäten, die als Bots identifiziert werden, haben &quot;Bot Activity&quot;als &quot;True&quot;und &quot;Bot Activity Pattern&quot;als identifiziertes Muster/Methode
* Aktivitäten, die als nicht &quot;bots&quot;gekennzeichnet sind, haben &quot;Bot Activity&quot;als &quot;False&quot;und &quot;Bot Activity Pattern&quot;als &quot;K/A&quot;.
* Aktivitäten, die vor der Einführung dieser Attribute stattgefunden haben, haben &quot;Bot Activity&quot;als &quot;&quot;(leer) und &quot;Bot Activity Pattern&quot;als &quot;&quot;(leer).

## Filtertyp auswählen {#select-filter-type}

1. Klicks **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicks **[!UICONTROL Email]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicken Sie auf **[!UICONTROL Bot-Aktivität]** Registerkarte.

   ![](assets/filtering-email-bot-activity-3.png)

1. Wählen Sie **[!UICONTROL Übereinstimmung mit IAB-Liste]**, **[!UICONTROL Übereinstimmung mit Näherungsmuster]** oder beides. Festlegen, ob [!UICONTROL Logbot-Aktivität] _oder_ [!UICONTROL Bot-Aktivität filtern].

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Wenn Sie [!UICONTROL Bot-Aktivität filtern]kann es zu einem Rückgang bei E-Mail-Öffnungen und Klicks kommen, da falsche Aktivitäten ausgeschaltet werden.

**OPTIONALER SCHRITT**: Um diese Funktion zu deaktivieren, deaktivieren Sie einfach die Schieberegler. Wenn Sie deaktivieren, werden die Daten nicht zurückgesetzt.

>[!TIP]
>
>Nutzen Sie Bot-Aktivitätsdaten in Smart-Listen über die booleschen Werte &quot;Is Bot Activity&quot;(Ja/Nein) und &quot;Bot Activity Pattern&quot;in den Filtern &quot;Clicked Link in Email&quot;und &quot;Open Email&quot;, sowie &quot;Clicks Link in Email&quot;und &quot;Opens Email&quot;.

## IP-Blockierungsliste {#ip-blocklist}

Wir haben eine Liste von IP-Adressen zusammengestellt, die für die Generierung von Millionen von gefälschten Interaktionen verantwortlich sind, da die Interaktion, die von einer der folgenden IPs empfangen wurde, automatisch herausgefiltert und nicht zu Ihrer Marketo Engage-Instanz hinzugefügt wird. Dies kann zu einer Verringerung von E-Mail-Öffnungen, Klicks und anderen damit zusammenhängenden Aktivitäten führen. Die nachstehende Liste kann regelmäßig aktualisiert werden.

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
* 209.222.82.126
* 209.222.82.127
* 209.222.82.128
* 209.222.82.129
* 209.222.82.138
* 209.222.82.139
* 209.222.82.140
* 209.222.82.141
* 209.222.82.228
* 209.222.82.229
* 209.222.82.230
* 209.222.82.231
* 209.222.82.232
* 209.222.82.233
* 209.222.82.234
* 209.222.82.235

>[!NOTE]
>
>Wir analysieren und überprüfen jede IP-Adresse sorgfältig, bevor sie dieser Liste hinzugefügt wird. Dadurch wird sichergestellt, dass nur die kritischsten und schädlichsten IP-Adressen blockiert werden.
