---
unique-page-id: 10098812
description: Einrichten der Umsatzzuordnung für digitale Advertising-Kampagnen - Marketo-Dokumente - Produktdokumentation
title: Einrichten der Umsatzzuordnung für Kampagnen des Typs „Digitales Advertising"
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Einrichten der Umsatzzuordnung für Kampagnen des Typs „Digitales Advertising&quot; {#set-up-revenue-attribution-for-digital-advertising-campaigns}

So richten Sie die Umsatzzuordnung für digitale Werbekanäle und -kampagnen ein. Nach der Einrichtung können Sie Umsätze für digitale Anzeigen per Erstkontakt und per Multi-Touch genauso zuordnen wie in anderen Marketo-Programmen.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Nachdem Sie Ihr erstes Anzeigenprogramm in Marketo eingerichtet haben, können Sie es klonen und für andere Kanäle aktualisieren. Klonen Sie beispielsweise ein LinkedIn-Programm in ein Facebook-Programm.

Mit separaten Programmen können Sie dann die Anzahl der Konversionen von jedem einzelnen verfolgen und Ihre Programme im Programm-Analyzer, im Opportunity-Einfluss-Analyzer und anderen Marketo Analytics-Funktionen sehen.

>[!PREREQUISITES]
>
>* Richten Sie ein Kanal-Tag mit Statuswerten und dem Programmerfolg ein (z. B. Digital Advertising oder Social Paid und PPC).
>* Erstellen oder bearbeiten Sie ein Formular, um eine Abfragezeichenfolge mit der Person zu übergeben
>* Stellen Sie sicher, dass Sie Zugriff auf einige Funktionen zur Umsatzzyklusanalyse haben, um Berichte über Ihre Anzeigenkanäle und Kampagnen zu erstellen

## Erstellen eines Standardprogramms {#create-a-default-program}

Im Gegensatz zu einigen Programmen (z. B. E-Mail), die gelegentlich über einen bestimmten Zeitraum ausgeführt werden, sind Standardprogramme immer aktiviert.

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Klicken Sie **Neu** und wählen Sie **Neues Programm**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Wenn Sie bereits über ein Programm verfügen, können Sie [klonen](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Achten Sie darauf, beim Klonen eines Programms die Namen in den Feldern der Abfragezeichenfolge der Smart-Listen zu ersetzen.

1. Platzieren Sie das neue Programm in einem bestimmten Kampagnenordner, nachdem das ursprüngliche Programm festgelegt wurde.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Eine über die URL übergebene Abfragezeichenfolge hilft Marketo dabei, zu erkennen, auf welche Anzeigenkampagne jemand geklickt hat, als er zu einer Person in Marketo wurde.
   >
   >Sie können eine Methodik für Abfragezeichenfolgen erstellen, die alle Variablen enthält, die Sie messen möchten. Marketo verwendet diese Variablen, um Personen zu Ihren verschiedenen Programmen hinzuzufügen.
   >
   >Sie können beispielsweise „channel_type_channel.asset__region__ verwenden. Dieser könnte wie folgt aussehen: SP_FB_NewGuide_US. **Hinweis**: Abkürzungen sparen Platz.
   >
   >Oder richten Sie sie als „Channel_Adsource_AssetName_Region_UniqueIdNumber“ ein. Das könnte wie folgt aussehen: Social-Paid_Facebook_NewGuide_NA_123.

## Erstellen einer Smart-Kampagne für neue Namen {#create-a-smart-campaign-for-new-names}

1. Erstellen Sie in der Smart-Kampagne eine Smart-Liste, die wie abgebildet zwei Trigger und zwei Filter enthält.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >Die in den beiden Triggern verwendete Abfragezeichenfolge und der Filter **Programm, das den Namen erfasst** sind für Sie eindeutig. Die hier gezeigten Abfragezeichenfolgen sind nur zum Beispiel. Wenn Sie das Feld geklont haben, ersetzen Sie einfach diese Felder.

1. Erstellen Sie einen Flussschritt, um das Attribut in **Akquise-Programm** zu ändern und den neuen Wert auf den Wert festzulegen, den Sie für bezahlte Social-Media-Kampagnen definiert haben.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Kampagne planen und aktivieren

## Erstellen einer Smart Campaign for Status/Program Success {#create-a-smart-campaign-for-status-program-success}

Sie benötigen eine zweite intelligente Kampagne, um den Status von Personen zu ändern, damit sie einen Programmerfolg erzielen und in die Berechnungen der Umsatzzuordnung einbezogen werden können.

1. Geben **im Trigger &quot;** Formular ausfüllen“ den Programmnamen in die Abfragezeichenfolge ein. Wenn Sie das Programm klonen, ersetzen Sie einfach den alten Namen der Abfragezeichenfolge durch den neuen.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Erstellen Sie Flussschritte, um den Status in einen zu ändern, der mit „Programm erfolgreich“ verknüpft ist.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >Das obige Beispiel zeigt **Konvertiert**, dies hängt jedoch von Ihren Status-/Erfolgswerten ab.

1. Kampagne planen und aktivieren

## Erstellen einer Anzeige {#create-your-ad}

Nachdem Sie das Programm und die Kampagnen eingerichtet haben, erstellen Sie die neue Anzeige.

1. Wechseln Sie zum -Kanal, z. B. LinkedIn oder Facebook.
1. Erstellen Sie eine neue Anzeige.
1. Wählen Sie eine Marketo-Landingpage als Ziel für den Aktionsaufruf in der Kampagne aus.
1. Fügen Sie die Abfragezeichenfolge zur URL hinzu.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >So können Sie alle von Ihnen eingerichteten Informationen zu einer tatsächlichen URL hinzufügen. Die Elemente werden durch ein kaufmännisches Und-Zeichen (&amp;) getrennt:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** ist die als Kanalkennung verwendete Personen-Source
   >* **Kommentar** ist die eindeutige Kennung, die für jedes Programm erstellt wird
   >* **CAMP** ist die Kampagne in Facebook, LinkedIn oder Google
   >* **KK** ist das Keyword oder der Asset-Name, den Sie erfassen möchten
   >
   >**Diese vier Begriffe müssen vollständig in Kleinbuchstaben geschrieben sein und die URL darf keine Leerzeichen enthalten, damit diese Informationen erfasst werden.**

## Bewährte Methoden {#best-practices}

Verwenden Sie ein einzelnes Kanal-Tag, um alle digitalen Advertising darzustellen, oder verwenden Sie mehrere Kanal-Tags, wenn Sie detailliertere Vergleiche mit Ihren anderen Marketing-Kanälen wünschen (z. B. Social-Paid, Search-Paid, Display, Retargeting).

Richten Sie dann für jede benötigte Berichtsansicht unterschiedliche Programme ein. Verwenden Sie eine gemeinsame ID als Parameter in der URL (z. B. BC) in der Abfragezeichenfolge, wenn Sie 10 Regionen haben, die zusammen eine „große Kampagne“ starten und Ergebnisse regionenübergreifend anzeigen möchten.

Wenn Sie über jede Region und die kollektiven Ergebnisse der großen Kampagne berichten möchten, erstellen Sie 11 Programme - eines für jede Region und eines für die große Kampagne. Jedes Programm verweist nur auf die relevanten Zeichen aus der Abfragezeichenfolge (z. B. BC).

Es gibt eine absichtliche Überschneidung bei der Personenzahl zwischen den Programmen der Big Campaign und der Region. Sie möchten also nicht über die Gesamtzahl der Personen in allen 11 Programmen berichten, da einige Personen sowohl in der Big Campaign als auch in einem der Programme der Region sind.
