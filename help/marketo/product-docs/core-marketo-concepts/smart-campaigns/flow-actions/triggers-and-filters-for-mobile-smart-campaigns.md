---
unique-page-id: 9437991
description: Trigger und Filter für mobile Smart-Kampagnen - Marketo-Dokumente - Produktdokumentation
title: Trigger und Filter für mobile Smart-Kampagnen
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 1%

---

# Trigger und Filter für mobile Smart-Kampagnen {#triggers-and-filters-for-mobile-smart-campaigns}

Sie können Trigger und Filter für eine App-Smart-Kampagne einrichten.

Bei den meisten Aktivitäten gibt es einen Trigger, einen Filter und einen Inaktivitätsfilter. Verwenden Sie Inaktivitätsfilter, um eine Aktion zu verfolgen, z. B. Tippen auf eine Push-Benachrichtigung, wenn _nicht_ aufgetreten ist.

* Die mobile App ist/wurde installiert
* Mobile App ist/wurde geöffnet
* Mobile App-Aktivität enthält/anzeigen
* Mobile App-Sitzung enthält/hatte
* Tippen/Tippen der mobilen Push-Benachrichtigung

Es gibt nur Filter für diese Aktivität:

* Wurde gesendet Push-Benachrichtigung - Filter und Inaktivitätsfilter

Suchen Sie im rechten Bereich nach &quot;mobile app&quot;, um alle Mobile App-Trigger und -Filter aufzulisten.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Einschränkungen {#constraints}

Verwenden Sie Einschränkungen mit Triggern und Filtern, um die Daten weiter zu sortieren.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Alle Trigger und Filter mit Ausnahme der Benachrichtigung über die gesendete Push-Benachrichtigung enthalten die folgenden beiden Standardeinschränkungen:

* Gerätetyp - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android Smartphone, Android Tablet, Unbekannt (dies ist eine voreingestellte Liste)

* Platform - iPhone oder Android

Einige Trigger und Filter bieten zusätzliche Einschränkungen wie:

* App-Version - Eine Möglichkeit, Personen anzusprechen, die nicht auf der neuesten Version basieren. Wenn die neueste App-Version beispielsweise 2.0 ist, können Sie sie verwenden, um Personen zu finden, die NICHT auf App Version 2.0 zugreifen.

* Source installieren - Derzeit ist die einzige Option die API

* Gebietsschema - Die Einstellung auf dem Gerät

* Mobile App - Der Name der jeweiligen App. Nützlich, um anzugeben, ob Sie mehr als eine

* Platform-Version - Die Version des Betriebssystems

* Sitzungslänge (Sekunden) - Sitzungszeit, wenn sich die App im Vordergrund befindet

* Ist Push-aktiviert - **True** bedeutet, dass Push-Benachrichtigungen gesendet werden können. **False** bedeutet, dass dies nicht möglich ist. Beispielsweise hat sich die Person vom Erhalt von Push-Benachrichtigungen abgemeldet.

## Trigger und Filter {#triggers-and-filters}

**Hat mobile App**

Verwenden Sie diesen Filter, um alle Personen herauszufinden, die Ihre App jemals installiert haben. Dies ist nur als Filter verfügbar.

>[!NOTE]
>
>Der Filter findet sowohl aktuelle als auch frühere Installationen, da Marketo App-Deinstallationen nicht verfolgt.

**Einschränkungen** - Gerätetyp, Plattform, mobile App, Version der mobilen App, Gerätetyp, Source installieren, Ist Push aktiviert und Gebietsschema

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>Es empfiehlt sich, bei der Definition der Smart-Liste der Empfänger einer Push-Benachrichtigung den Wert Hat Mobile App = true und Ist Push aktiviert = true sowie den Namen Ihrer Mobile App anzugeben.

Die mobile App ist/wurde installiert

* Mobile App ist installiert - Trigger

* Mobile App wurde installiert - Filter

* NOT Mobile App wurde installiert - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp, Plattform, App-Version, Gebietsschema und Installation von Source

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

Mobile App ist/wurde geöffnet

* Mobile App ist geöffnet - Trigger

* Mobile App wurde geöffnet - Filter

* NOT Mobile App wurde geöffnet - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp und Plattform

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Mobile App-Aktivität enthält/anzeigen

Diese bieten eine leistungsstarke Möglichkeit, benutzerdefinierte mobile Aktivitäten zu verfolgen. Sie müssen mit Ihrem Entwickler zusammenarbeiten, um das Tracking [für Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android){target="_blank"} und [für iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios){target="_blank"} einzurichten.

* Mobile App-Aktivität - Trigger

* Handy-App-Aktivität anzeigen - Filter

* NICHT über Mobile-App-Aktivität verfügen - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp, Plattform, Mobile App-Version, Gebietsschema, Plattformversion plus fünf weitere:

* Aktion - Benutzerdefinierte mobile Aktivität

* Aktionstyp - (optional) Textfeld, das zur Kategorisierung mehrerer Aktionen verwendet wird

* Aktionsdetails - (optional) Textfeld mit zusätzlichen Informationen zu einer Aktion

* Aktionsmetrik - (optional) Numerisches Feld, das zusätzliche Informationen zu einer Aktion bereitstellt (z. B. Preis)

* Aktionslänge (Sekunden) - (optional) Numerisches Feld, mit dem erfasst werden kann, wie lange ein Benutzer für die Durchführung einer Aktion gebraucht hat

Mit den Aktionsbegrenzungen können Sie den Trigger und Filter sehr genau verwenden, um mobile Aktivitäten zu verfolgen.

>[!NOTE]
>
>**Beispiel**
>
>Unter dem Aktionstyp *Shopping* finden Sie hier eine sehr spezifische Aktion, die durch die anderen Einschränkungen definiert wird:
>
>* Ein Hemd gekauft
>   * Es war rot
>   * Es hat 30 Dollar gekostet
>   * Der Kauf dauerte 20 Sekunden

So sieht der Filter in Marketo aus:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Beispiel**
>
>Sie können mehrere Aktionen unter demselben Aktionstyp haben. In der Tat kann Ihr normales Einkaufserlebnis mehrere Spalten unter Shopping! Wie wäre es mit ein paar Socken, die dazu passen?
>
>| Aktionstyp | Shopping | Shopping |
>|---|---|---|
>| Aktion | Gepäck-Shirt | Gepackte Hosen |
>| Aktionsdetails | Farbe | Farbe |
>| Aktionsmetrik | Preis | Preis |

**Hat/hatte Mobile App-Sitzung**

* Hat mobile App-Sitzung - Trigger

* Mobile-App-Sitzung - Filter

* NOT Had Mobile App Session - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp, Plattform und Sitzungslänge (Sekunden)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Tippen/Tippen-Push-Benachrichtigung

* Tips Push Notification - Trigger

* Getippte Push-Benachrichtigung - Filter

* NOT Tapped Push Notification - Inactivity filter

**Einschränkungen** - Gerätetyp, Plattform, Version der mobilen App, Push-Benachrichtigung und Plattformversion

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Verwenden Sie den Filter Nicht getippte Push-Benachrichtigung , um Personen zu finden, die nicht auf eine Push-Benachrichtigung getippt haben, die ihnen kürzlich gesendet wurde. So können Sie per E-Mail Folgemaßnahmen durchführen.

**Wurde Push-Benachrichtigung gesendet** Diese Aktivität ist nur als Filter verfügbar.

* Wurde gesendet Push-Benachrichtigung - Filter

* NOT WURDE Push-Benachrichtigung gesendet - Inaktivitätsfilter

**Einschränkungen** - Push-Benachrichtigung und mobile App

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Eine Beschränkung zu einem Smart-List-Filter hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}
>* [Verwenden von Inaktivitätsfiltern in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
