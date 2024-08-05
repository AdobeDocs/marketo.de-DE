---
unique-page-id: 10098812
description: Einrichten der Umsatzzuordnung für digitale Advertising-Kampagnen - Marketo Docs - Produktdokumentation
title: Einrichten der Umsatzzuordnung für digitale Advertising-Kampagnen
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Einrichten der Umsatzzuordnung für digitale Advertising-Kampagnen {#set-up-revenue-attribution-for-digital-advertising-campaigns}

So richten Sie die Umsatzzuordnung für digitale Werbekanäle und Kampagnen ein. Nach der Einrichtung können Sie die Erstkontakt- und Multi-Touch-Umsatzzuordnung für digitale Anzeigen auf die gleiche Weise vornehmen wie bei anderen Marketo-Programmen.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Sie können keine neuen Assets erstellen. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Nachdem Sie Ihr erstes Werbeprogramm in Marketo eingerichtet haben, können Sie es klonen und für andere Kanäle aktualisieren. Klonen Sie beispielsweise ein LinkedIn-Programm auf ein Facebook-Programm.

Mit separaten Programmen können Sie dann die Anzahl der Konversionen von jedem einzelnen verfolgen und Ihre Programme in Programm Analyzer, Opportunity Influence Analyzer und anderen Marketo Analytics-Funktionen anzeigen.

>[!PREREQUISITES]
>
>* Einrichten eines Kanal-Tags mit Statuswerten und Programmerfolg (z. B. Digital Advertising oder Social Paid und PPC)
>* Erstellen oder bearbeiten Sie ein Formular, um eine Abfragezeichenfolge an die Person weiterzugeben
>* Stellen Sie sicher, dass Sie Zugriff auf einige Analytics-Funktionen von Umsatzzyklen haben, um Berichte zu Ihren Anzeigenkanälen und -kampagnen zu erstellen.

## Standardprogramm erstellen {#create-a-default-program}

Im Gegensatz zu einigen Programmen (wie E-Mails), die für einen bestimmten Zeitraum regelmäßig ausgeführt werden, sind Standardprogramme immer aktiviert.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neues Programm** aus.

   ![](assets/image2016-3-14-15-52-0.png)

1. Wenn Sie bereits ein Programm eingerichtet haben, können Sie [es klonen](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Wenn Sie ein Programm klonen, müssen Sie die Namen in den Abfragezeichenfolgenfeldern der Smart-Listen ersetzen.

1. Platzieren Sie das neue Programm in einen bestimmten Kampagnenordner, nachdem das ursprüngliche Programm festgelegt wurde.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Eine Abfragezeichenfolge, die über die URL übergeben wird, hilft Marketo dabei zu wissen, auf welche Anzeigenkampagne jemand geklickt hat, als er in Marketo eine Person wurde.
   >
   >Sie können eine Abfragezeichenfolgenmethodik erstellen, die alle Variablen enthält, die Sie messen möchten. Marketo verwendet diese Variablen, um Ihren verschiedenen Programmen Personen hinzuzufügen.
   >
   >Sie können beispielsweise Kanal type_Channel__Asset__Region verwenden. Dies könnte wie folgt aussehen: SP_FB_NewGuide_US. **Hinweis**: Abkürzungen sparen Platz.
   >
   >Oder richten Sie es als Channel_Adsource_AssetName_Region_UniqueIdNumber ein. Das könnte wie folgt aussehen: Social-Paid_Facebook_NewGuide_NA_123.

## Erstellen einer Smart-Kampagne für neue Namen {#create-a-smart-campaign-for-new-names}

1. Erstellen Sie in der Smart-Kampagne eine Liste mit zwei Triggern und zwei Filtern, wie in der Abbildung dargestellt.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >Die in den beiden Triggern verwendete Abfragezeichenfolge und der Filter **Programm, das den erfassten Namen** enthält, sind für Sie eindeutig. Die hier gezeigten Abfragezeichenfolgen sind beispielsweise nur verfügbar. Wenn Sie das Feld geklont haben, ersetzen Sie einfach diese Felder.

1. Erstellen Sie einen Flussschritt, um das Attribut in **Akquise-Programm** zu ändern und den neuen Wert auf den Wert festzulegen, den Sie für gebührenpflichtige Social-Media-Kampagnen definiert haben.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Planen und aktivieren Sie die Kampagne.

## Erstellen einer Smart-Kampagne für Status-/Programmerfolg {#create-a-smart-campaign-for-status-program-success}

Sie benötigen eine zweite intelligente Kampagne, um den Status von Personen zu ändern, damit diese den Programmerfolg erzielen und in die Berechnung der Umsatzzuordnung einbezogen werden können.

1. Geben Sie im Trigger **Formular ausfüllen** den Programmnamen in die Abfragezeichenfolge ein. Wenn Sie das Programm klonen, ersetzen Sie einfach den alten Namen der Abfragezeichenfolge durch den neuen.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Erstellen Sie Workflow-Schritte, um den Status in einen Status zu ändern, der mit dem Programmerfolg verknüpft ist.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >Das obige Beispiel zeigt **Konvertiert**, dies hängt jedoch von Ihren Status-/Erfolgswerten ab.

1. Planen und aktivieren Sie die Kampagne.

## Erstellen Ihrer Anzeige {#create-your-ad}

Nachdem Sie das Programm und die Kampagnen eingerichtet haben, erstellen Sie die neue Anzeige.

1. Wechseln Sie zum Kanal, z. B. LinkedIn oder Facebook.
1. Erstellen Sie eine neue Anzeige.
1. Wählen Sie eine Marketo-Landingpage als Ziel für den Aktionsaufruf in der Kampagne aus.
1. Fügen Sie die Abfragezeichenfolge zur URL hinzu.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >So können Sie alle von Ihnen eingerichteten Informationen zu einer tatsächlichen URL hinzufügen. Die Elemente werden durch ein kaufmännisches Und-Zeichen (&amp;) voneinander getrennt:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** ist die Person, die von Source als Kanalkennung verwendet wird.
   >* **comment** ist die eindeutige Kennung, die für jedes Programm erstellt wird.
   >* **camp** ist die Kampagne in Facebook, LinkedIn oder Google
   >* **kk** ist das Keyword oder der Asset-Name, das/die Sie erfassen möchten
   >
   >**Diese vier Begriffe müssen in Kleinbuchstaben verfasst sein, und die URL darf keine Leerzeichen enthalten, damit diese Informationen erfasst werden.**

## Bewährte Methoden {#best-practices}

Verwenden Sie ein einzelnes Kanal-Tag, um alle Digital Advertising-Tags darzustellen, oder mehrere Kanal-Tags, wenn Sie detailliertere Vergleiche mit Ihren anderen Marketing-Kanälen wünschen (z. B. Social-Paid, Search-Paid, Display, Retargeting).

Richten Sie dann für jede benötigte Berichtsansicht verschiedene Programme ein. Verwenden Sie eine allgemeine ID als Parameter in der URL (z. B. BC) in der Abfragezeichenfolge, wenn 10 Regionen eine &quot;Big Campaign&quot;gemeinsam starten und Ergebnisse regionsübergreifend anzeigen möchten.

Wenn Sie über jede Region und die gemeinsamen Ergebnisse der Big Campaign berichten möchten, erstellen Sie 11 Programme - eines für jede Region und eines für die Big Campaign. Jedes Programm verweist nur auf die relevanten Zeichen aus der Abfragezeichenfolge (z. B. BC).

Es gibt absichtliche Überschneidungen bei der Personenzahl zwischen den Programmen &quot;Big Campaign&quot;und &quot;Region&quot;, sodass Sie nicht über die Gesamtzahl der Menschen in allen 11 Programmen berichten möchten, da einige Personen sowohl in der Big Campaign-Kampagne als auch in einem der Programme der Region sind.
