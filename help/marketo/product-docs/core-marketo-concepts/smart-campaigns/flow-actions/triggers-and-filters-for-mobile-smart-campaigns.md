---
unique-page-id: 9437991
description: Auslöser und Filter für mobile intelligente Kampagnen - Marketing Docs - Produktdokumentation
title: Auslöser und Filter für mobile intelligente Kampagnen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


# Auslöser und Filter für mobile intelligente Kampagnen {#triggers-and-filters-for-mobile-smart-campaigns}

Sie können Auslöser und Filter für eine mobile App-Kampagne einrichten.

Für die meisten Aktivitäten gibt es einen Auslöser, einen Filter und einen Inaktivitätsfilter. Verwenden Sie Inaktivität-Filter, um eine Aktion zu verfolgen, z. B. Tippen auf eine Push-Benachrichtigung, dass *nicht* stattgefunden hat.

* Mobile App ist installiert/wurde installiert
* Mobile App wurde geöffnet
* Hat/hat eine mobile App-Aktivität
* Hat/hat Mobile App-Sitzung
* Tippen/Tippen-Push-Benachrichtigung für Mobilgeräte

Es gibt nur Filter für diese Aktivität:

* Push-Benachrichtigung gesendet - Filter- und Inaktivitätsfilter

Suchen Sie im rechten Bereich nach **Mobil-App**, um alle Mobile App-Auslöser und -Filter Liste.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Einschränkungen {#constraints}

Verwenden Sie Einschränkungen mit Auslösern und Filtern, um die Daten weiter zu sortieren.

![](assets/image2015-8-17-12-3a6-3a33.png)

Alle Auslöser und Filter mit Ausnahme der Benachrichtigung zum Versand der Push-Benachrichtigung enthalten die folgenden beiden Standardeinschränkungen:

* Gerätetyp - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android-Smartphone, Android-Tablet, Unbekannt (dies ist eine voreingestellte Liste)

* Plattform - iPhone oder Android

Einige Auslöser und Filter haben zusätzliche Einschränkungen zum Angebot:

* App-Version - Eine Möglichkeit zur Zielgruppe von Personen, die nicht die neueste Version verwenden. Wenn die neueste App-Version beispielsweise 2.0 ist, können Sie sie verwenden, um Personen zu suchen, die NICHT in App Version 2.0 arbeiten.

* Installationsquelle - Derzeit ist die einzige Option die API

* Gebietsschema - Die Einstellung auf dem Gerät

* Mobile App - Der Name einer bestimmten App. Nützlich, um anzugeben, ob Sie mehr als eine

* Plattformversion - Die Version des Betriebssystems

* Sitzungslänge (Sekunden) - Sitzungszeit, wenn die App im Vordergrund steht

* Ist Push-aktiviert - **True** bedeutet, dass Push-Benachrichtigungen gesendet werden können. **** Falsemeans, die sie nicht können; die Person hat sich beispielsweise vom Empfang von Push-Benachrichtigungen abgemeldet

## Auslöser und Filter {#triggers-and-filters}

**Hat mobile Anwendung**

Verwenden Sie diesen Filter, um alle Personen herauszufinden, die Ihre App jemals installiert haben. Dies ist nur als Filter verfügbar.

>[!NOTE]
>
>Der Filter findet sowohl aktuelle als auch frühere Installationen, da Marketo keine App-Deinstallationen verfolgt.

**Einschränkungen**: Gerätetyp, Plattform, mobile Anwendung, Version der mobilen Anwendung, Gerätetyp, Installationsquelle, Ist Push-aktiviert und Gebietsschema

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>Es empfiehlt sich, beim Definieren der intelligenten Liste, wer eine Push-Benachrichtigung erhalten soll, sowohl den Namen der mobilen App als auch den Namen der App als true festzulegen.

Mobile App ist installiert/wurde installiert

* Mobile App ist installiert - Trigger

* Mobile App wurde installiert - Filter

* NOT Mobile App wurde installiert - Inaktivitätsfilter

**Einschränkungen**: Gerätetyp, Plattform, App-Version, Gebietsschema und Installationsquelle

![](assets/image2015-8-17-13-3a11-3a3.png)

Mobile App wurde geöffnet

* Mobile App wird geöffnet - Auslöser

* Mobile App wurde geöffnet - Filter

* NOT Mobile App wurde geöffnet - Inaktivitätsfilter

**Einschränkungen**: Gerätetyp und Plattform

![](assets/image2015-8-17-13-3a13-3a55.png)

Hat/hat eine mobile App-Aktivität

Diese bieten eine leistungsstarke Möglichkeit, benutzerdefinierte mobile Aktivitäten zu verfolgen. Sie müssen mit Ihrem Entwickler zusammenarbeiten, um die Verfolgung [für Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android) und [für iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios) einzurichten.

* Hat Aktivität für mobile Anwendung - Auslöser

* Aktivität der mobilen App - Filter

* AKTIVITÄT der mobilen App NICHT verfügbar - Inaktivitätsfilter

**Einschränkungen**: Gerätetyp und Plattform sowie fünf weitere:

* Aktion - Benutzerspezifische mobile Aktivität

* Aktionstyp - (optional) Textfeld zur Kategorisierung mehrerer Aktionen

* Aktionsdetails - (optional) Textfeld mit zusätzlichen Informationen zu einer Aktion

* Aktionsmetrik - (optional) Numerisches Feld mit zusätzlichen Informationen zu einer Aktion (z. B. Preis)

* Aktionslänge (Sekunden) - (optional) Numerisches Feld, mit dem erfasst werden kann, wie lange ein Benutzer eine Aktion durchgeführt hat

Mit den Aktionsbeschränkungen können Sie Auslöser und Filter verwenden, um die mobile Aktivität sehr genau zu verfolgen.

>[!NOTE]
>
>**Beispiel**
>
>Unter dem Aktionstyp *Shopping* gibt es eine sehr spezifische Aktion, die durch die anderen Beschränkungen definiert wird:
>
>* Hemd gekauft
>  * Es war rot
>  * Es kostet 30 Dollar
>  * Der Kauf dauerte 20 Sekunden


So sieht der Filter in Marketo aus:   ![](assets/image2015-8-17-13-3a16-3a12.png)

>[!NOTE]
>
>**Beispiel**
>
>Sie können mehrere Aktionen unter demselben Aktionstyp ausführen. In der Tat Ihr normales Einkaufserlebnis kann mehrere Spalten unter Einkaufen! Wie wäre es mit ein paar Socken, die damit einhergehen?
>
>| Aktionstyp | Einkauf | Einkauf |
>|---|---|---|
>| Aktion | Einkaufshirt | Gepuftete Hosen |
>| Aktionsdetails | Farbe | Farbe |
>| Aktionsmetrik | Preis | Preis |


**Hat/hat Mobile App-Sitzung**

* Hat Mobile App Session - Trigger

* Habe Mobile App Session - Filter

* Mobile App-Sitzung NICHT abgeschlossen - Inaktivitätsfilter

**Einschränkungen**: Gerätetyp, Plattform und Sitzungslänge (Sekunden)

![](assets/image2015-8-17-13-3a18-3a34.png)

Tippen/Tippen-Push-Benachrichtigung

* Tips-Push-Benachrichtigung - Auslöser

* Tippen - Push-Benachrichtigung - Filter

* NICHT getippte Push-Benachrichtigung - Inaktivitätsfilter

**Einschränkungen**: Gerätetyp, Plattform, Version der mobilen App, Push-Benachrichtigung und Plattformversion

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Verwenden Sie den Filter &quot;Nicht getippte Push-Benachrichtigung bei Inaktivität&quot;, um nach Personen zu suchen, die nicht auf eine Push-Benachrichtigung tippen, die ihnen vor kurzem gesendet wurde, damit Sie per E-Mail nachverfolgen können.

**Push-** Benachrichtigung gesendetDiese Aktivität ist nur als Filter verfügbar.

* Push-Benachrichtigung gesendet - Filter

* KEINE Push-Benachrichtigung gesendet - Inaktivitätsfilter

**Einschränkungen**: Push-Benachrichtigung und mobile App

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!MORELIKETHIS]
>
>* [hinzufügen einer Beschränkung auf einen Filter für intelligente Listen](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Inaktive Filter in einer intelligenten Liste verwenden](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

