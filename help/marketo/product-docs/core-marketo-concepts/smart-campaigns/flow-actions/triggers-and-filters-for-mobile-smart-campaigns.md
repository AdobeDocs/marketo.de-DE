---
unique-page-id: 9437991
description: Trigger und Filter für Smart-Mobile-Kampagnen - Marketo-Dokumente - Produktdokumentation
title: Trigger und Filter für Smart-Kampagnen für Mobilgeräte
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%

---

# Trigger und Filter für Smart-Kampagnen für Mobilgeräte {#triggers-and-filters-for-mobile-smart-campaigns}

Sie können Trigger und Filter für eine Smart-Kampagne für Mobile Apps einrichten.

Für die meisten Aktivitäten gibt es einen Trigger, einen Filter und einen Inaktivitätsfilter. Verwenden Sie Inaktivitätsfilter, um eine Aktion nachzuverfolgen, z. B. auf eine Push-Benachrichtigung zu tippen _die_ stattgefunden hat.

* Mobile App ist/war installiert
* Mobile App ist/wurde geöffnet
* Hat/hatte die Aktivität „Mobile App“
* Hat/hatte Mobile-App-Sitzung
* Tippen/tippen Sie auf Mobile Push-Benachrichtigung

Es gibt nur Filter für diese Aktivität:

* Push-Benachrichtigung gesendet - Filter und Inaktivitätsfilter

Suchen Sie im rechten Bereich nach „Mobile App“, um alle Trigger und Filter der Mobile App aufzulisten.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Begrenzungen {#constraints}

Verwenden Sie Einschränkungen mit Triggern und Filtern, um die Daten weiter zu sortieren.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Alle Trigger und Filter mit Ausnahme der Push-Benachrichtigung „wurde gesendet“ enthalten diese beiden Standardeinschränkungen:

* Gerätetyp - [!DNL iPod], iPhone, [!DNL iPhone 6 Plus], [!DNL iPad mini], iPad, Android Smartphone, Android Tablet, Unbekannt (dies ist eine Voreinstellungsliste)

* Platform - iPhone oder Android

Einige Trigger und Filter bieten zusätzliche Einschränkungen, z. B.:

* App-Version - Eine Möglichkeit, Personen anzusprechen, die nicht die neueste Version verwenden. Wenn die neueste App-Version beispielsweise 2.0 ist, können Sie damit nach Personen suchen, die NICHT in der App-Version 2.0 sind

* Source installieren - Derzeit ist die einzige Option die API

* Gebietsschema : Die Einstellung auf dem Gerät

* Mobile App : Der Name der bestimmten App. Nützlich, um anzugeben, wenn mehrere vorhanden sind

* Plattformversion - Die Version des Betriebssystems

* Sitzungsdauer (Sekunden) - Sitzungsdauer, während der sich die Mobile App im Vordergrund befindet

* Ist Push-Benachrichtigung aktiviert - **True** bedeutet, dass Push-Benachrichtigungen gesendet werden können. **False** bedeutet, dass dies nicht möglich ist. Beispielsweise könnte die Person den Erhalt von Push-Benachrichtigungen abgelehnt haben

## Trigger und Filter {#triggers-and-filters}

**Hat Mobile App**

Verwenden Sie diesen Filter, um alle Personen herauszufinden, die Ihre App schon einmal installiert haben. Dies ist nur als Filter verfügbar.

>[!NOTE]
>
>Der Filter findet sowohl aktuelle als auch frühere Installationen, da Marketo keine App-Deinstallationen verfolgt.

**Einschränkungen** - Gerätetyp, Plattform, Mobile App, Mobile App-Version, Gerätetyp, Source installieren, Push-Benachrichtigung aktiviert und Gebietsschema

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>Es empfiehlt sich, bei der Definition der Smart-Liste der Personen, die eine Push-Benachrichtigung erhalten sollen, anzugeben, dass die Mobile App den Wert „true“ und die Push-Benachrichtigung den Wert „true“ hat sowie den Namen der Mobile App.

Mobile App ist/war installiert

* Mobile App ist installiert - Trigger

* Mobile App wurde installiert - Filter

* NOT Mobile App was Installed - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp, Plattform, App-Version, Gebietsschema und Source installieren

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

Mobile App ist/wurde geöffnet

* Mobile App ist geöffnet - Trigger

* Mobile App wurde geöffnet - Filter

* NOT Mobile App was Opened - Inaktivitätsfilter

**Beschränkungen** - Gerätetyp und Plattform

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Hat/hatte die Aktivität „Mobile App“

Diese bieten eine leistungsstarke Möglichkeit, benutzerdefinierte mobile Aktivitäten zu verfolgen. Sie müssen mit Ihrem Entwickler zusammenarbeiten, um das Tracking ([ Android) ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android){target="_blank"} ([ iOS) ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios){target="_blank"}.

* Hat Mobile-App-Aktivität - Trigger

* Mobile-App-Aktivität - Filter

* Mobile-App-Aktivität NICHT vorhanden - Inaktivitätsfilter

**Beschränkungen** - Gerätetyp, Plattform, Mobile-App-Version, Gebietsschema, Plattform-Version plus fünf zusätzliche:

* Aktion - Benutzerdefinierte mobile Aktivität

* Aktionstyp : (Optional) Ein Textfeld, mit dem mehrere Aktionen kategorisiert werden.

* Aktionsdetails (optional): Ein Textfeld, das zusätzliche Informationen zu einer Aktion bereitstellt

* Aktionsmetrik (optional): Ein numerisches Feld, das zusätzliche Informationen zu einer Aktion bereitstellt (z. B. Preis).

* Aktionslänge (Sekunden) - (optional) Ein numerisches Feld, mit dem erfasst werden kann, wie lange ein Benutzer für die Durchführung einer Aktion gebraucht hat

Mithilfe der Aktionseinschränkungen können Sie den Trigger und die Filter verwenden, um mobile Aktivitäten sehr genau zu verfolgen.

>[!NOTE]
>
>**Beispiel**
>
>Unter dem Aktionstyp _Shopping_ befindet sich eine sehr spezifische Aktion, die durch die anderen Einschränkungen definiert wird:
>
>* Ich habe ein Hemd gekauft
>   * Es war rot
>   * Es kostete 30 Dollar
>   * Der Kauf dauerte 20 Sekunden

So sieht der Filter in Marketo aus:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Beispiel**
>
>Sie können mehrere Aktionen unter demselben Aktionstyp haben. Tatsächlich kann Ihr normales Einkaufserlebnis mehrere Spalten unter „Shopping“ umfassen! Wie wäre es mit ein paar Socken dazu?
>
>| Aktionstyp | Einkaufen | Einkaufen |
>|---|---|---|
>| Aktion | gekauftes Hemd | gekaufte Hose |
>| Aktionsdetails | Farbe | Farbe |
>| Aktionsmetrik | Preis | Preis |

**Hat/hatte Mobile-App-Sitzung**

* Hat Mobile-App-Sitzung - Trigger

* Had Mobile App Session - Filter

* NOT Had Mobile App Session - Inaktivitätsfilter

**Beschränkungen** - Gerätetyp, Plattform und Sitzungslänge (Sekunden)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Tippen/Tippen auf Push-Benachrichtigung

* Tippen auf Push-Benachrichtigung - Trigger

* Push-Benachrichtigung angetippt - Filter

* NICHT auf Push-Benachrichtigung getippt - Inaktivitätsfilter

**Einschränkungen** - Gerätetyp, Plattform, Mobile-App-Version, Push-Benachrichtigung und Platform-Version

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Verwenden Sie den Filter Inaktivität für nicht getippte Push-Benachrichtigungen , um Personen zu finden, die nicht auf eine kürzlich an sie gesendete Push-Benachrichtigung getippt haben, damit Sie per E-Mail weiterarbeiten können.

**Push-Benachrichtigung wurde gesendet** Diese Aktivität ist nur als Filter verfügbar.

* Push-Benachrichtigung gesendet - Filter

* NICHT gesendet Push-Benachrichtigung - Inaktivitätsfilter

**Einschränkungen** - Push-Benachrichtigung und Mobile App

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Fügen Sie eine Einschränkung zu einem Smart-Listen-Filter hinzu](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}
>* [Verwenden von Inaktivitätsfiltern in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
