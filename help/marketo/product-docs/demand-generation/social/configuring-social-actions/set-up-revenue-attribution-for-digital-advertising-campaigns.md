---
unique-page-id: 10098812
description: Einrichten der Umsatzzuordnung für Digital Advertising Kampagnen - Marketing Docs - Produktdokumentation
title: Einrichten der Umsatzzuordnung für Digital Advertising-Kampagnen
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Einrichten der Umsatzzuordnung für Digital Advertising Kampagnen {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Hier sehen Sie, wie Sie die Umsatzzuordnung für Kanal und Kampagnen digitaler Werbung einrichten. Nach der Einrichtung können Sie für digitale Anzeigen First Touch- und Multi-Touch-Umsätze auf die gleiche Weise wie in anderen Marketo-Programmen zuordnen.

Nachdem Sie Ihr erstes Programm in Marketo eingerichtet haben, können Sie es klonen und für andere Kanal aktualisieren. Klonen Sie beispielsweise ein LinkedIn-Programm mit einem Facebook-Element.

Mit separaten Programmen können Sie dann die Anzahl der Konvertierungen aus jedem  verfolgen und Ihre Programm in Programm Analyzer, Opportunity Influence Analyzer und anderen Marketingto Analytics-Funktionen anzeigen.

>[!PREREQUISITES]
>
>* Richten Sie ein Kanal-Tag mit Statuswerten und Programm-Erfolg ein (z. B. Digital Advertising oder Social Paid und PPC)
>* Erstellen oder bearbeiten Sie ein Formular, um eine Abfrage-Zeichenfolge mit der Person zu übergeben
>* Vergewissern Sie sich, dass Sie Zugriff auf einige Analytics-Funktionen von &quot;Umsatz&quot;haben, um Berichte zu Ihren Kanälen und Kampagnen der Anzeige zu erstellen.


## Erstellen eines Standard-Programms {#create-a-default-program}

Im Gegensatz zu einigen Programmen (z. B. E-Mail), die für einen bestimmten Zeitraum in regelmäßigen Abständen ausgeführt werden, sind die standardmäßigen Programm immer aktiviert.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neues Programm**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Wenn Sie bereits ein Programm eingerichtet haben, können Sie [es klonen](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Wenn Sie ein Programm klonen, müssen Sie die Namen in den Abfragen-Zeichenfolgenfeldern der intelligenten Listen ersetzen.

1. Platzieren Sie das neue Programm in einem bestimmten Kampagnen-Ordner, nachdem das erste Programm festgelegt wurde.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Eine Abfrage-Zeichenfolge, die über die URL weitergegeben wird, hilft Marketo zu wissen, auf welche Kampagne eine Person geklickt hat, als sie in Marketo tätig wurde.
   >
   >Sie können eine Abfrage-Zeichenfolgenmethodik erstellen, die alle zu messenden Variablen enthält. Marketo verwendet diese Variablen, um Personen zu Ihren verschiedenen Programmen hinzuzufügen.
   >
   >Sie können beispielsweise Kanal type_Kanal__Asset__Region verwenden. Das könnte so aussehen: SP_FB_NewGuide_US. **Hinweis**: Abkürzungen sparen Platz.
   >
   >Sie können es auch als Kanal_Adsource_AssetName_Region_UniqueIdNumber einrichten. Das könnte so aussehen: Social-Paid_Facebook_NewGuide_NA_123.

## Erstellen einer intelligenten Kampagne für neue Namen {#create-a-smart-campaign-for-new-names}

1. Erstellen Sie in der intelligenten Kampagne eine intelligente Liste, die, wie gezeigt, zwei Trigger und zwei Filter enthält.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >Die in den beiden Triggern verwendete Zeichenfolge für die Abfrage und der Filter **Programm, das den erfassten Namen** erfasst hat, sind für Sie eindeutig. Die hier gezeigten Abfragen-Zeichenfolgen sind beispielsweise nur verfügbar. Wenn Sie das Feld geklont haben, ersetzen Sie einfach diese Felder.

1. Erstellen Sie einen Flussschritt, um das Attribut in **Akquise-Programm** zu ändern, und legen Sie den Neuen Wert auf den Wert fest, den Sie für gebührenpflichtige Social-Kampagnen definiert haben.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Planen und aktivieren Sie die Kampagne.

## Erstellen einer intelligenten Kampagne für Status-/Programm-Erfolg {#create-a-smart-campaign-for-status-program-success}

Sie benötigen eine zweite intelligente Kampagne, um den Status von Personen zu ändern, damit sie Programm erfolgreich erzielen und in Umsatzzuordnungsberechnungen einbezogen werden können.

1. Geben Sie im Trigger **Ausfüllen des Formulars** den Programm in die Abfrage ein. Wenn Sie das Programm klonen, ersetzen Sie einfach den alten Abfragen-Zeichenfolgennamen durch den neuen.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Erstellen Sie die Flussschritte, um den Status in einen Status zu ändern, der mit dem Erfolg des Programms verknüpft ist.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >Das obige Beispiel zeigt **Konvertiert**, aber dies hängt von Ihren Status-/Erfolgswerten ab.

1. Planen und aktivieren Sie die Kampagne.

## Erstellen Ihrer Anzeige {#create-your-ad}

Nachdem Sie das Programm und die Kampagnen eingerichtet haben, erstellen Sie die neue Anzeige.

1. Geh zum Kanal; z. B. LinkedIn oder Facebook.
1. Erstellen Sie eine neue Anzeige.
1. Wählen Sie eine Marketing-Landingpage als Ziel für den Aktionsaufruf in der Kampagne aus.
1. hinzufügen die Abfrage-Zeichenfolge der URL.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >So können Sie alle von Ihnen eingerichteten Informationen zu einer tatsächlichen URL hinzufügen. Die Elemente werden durch ein kaufmännisches Und (&amp;) getrennt:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **** Quellen der als Kanal-ID verwendeten Personenquelle
   >* **Der für jedes Programm erstellte eindeutige Bezeichner** kommentiert
   >* **&quot;** campis&quot;ist die Kampagne in Facebook, LinkedIn oder Google
   >* **** kkkis der Suchbegriff oder Asset-Name, den Sie erfassen möchten

   >
   >**Diese vier Begriffe müssen klein geschrieben sein, und es dürfen keine Leerzeichen in der URL vorhanden sein, damit diese Informationen erfasst werden.**

## Best Practices {#best-practices}

Verwenden Sie ein einzelnes Kanal-Tag zur Darstellung aller digitalen Werbung oder mehrere Kanal-Tags, wenn Sie genauere Vergleiche mit anderen Marketing-Kanälen anstellen möchten (z. B. Social-Paid, Search-Paid, Display, Retargeting).

Richten Sie dann für jede Berichte-Ansicht, die Sie benötigen, unterschiedliche Programm ein. Verwenden Sie eine allgemeine ID als Parameter in der URL (z. B. BC) in der Abfrage-Zeichenfolge, wenn 10 Regionen eine &quot;Große Kampagne&quot;gemeinsam starten und die Ergebnisse regionsübergreifend Ansicht werden sollen.

Wenn Sie über jede Region und die kollektiven Ergebnisse der Großen Kampagne berichten möchten, erstellen Sie elf Programme - eines für jede Region und eines für die Große Kampagne. Jedes Programm verweist nur auf die relevanten Zeichen aus der Abfrage (z. B. BC).

Es gibt absichtliche Überschneidungen bei der Personenzahl zwischen den Programmen der Großen Kampagne und der Region, sodass Sie nicht über die Gesamtanzahl der Menschen in allen 11 Programmen berichten möchten, da einige Menschen sowohl in der Großen Kampagne als auch in einem der Programme der Region leben.
