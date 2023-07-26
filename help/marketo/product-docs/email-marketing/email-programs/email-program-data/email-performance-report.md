---
unique-page-id: 2359467
description: E-Mail-Leistungsbericht - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Leistungsbericht
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# E-Mail-Leistungsbericht {#email-performance-report}

Erstellen Sie einen E-Mail-Leistungsbericht, um zu sehen, wie gut Ihre E-Mails mit Statistiken wie Zugestellt, Öffnungen, Klicks usw. funktionieren.

1. [Erstellen eines Berichts in einem Programm](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) und wählen Sie die **E-Mail-Leistung** [Berichtstyp](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändern des Berichtszeitrahmens](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) und klicken Sie auf **Bericht** Registerkarte.
1. Du bist da! Sehen Sie sich nun den Bericht an, um zu sehen, wie Ihre E-Mails abgeschnitten haben.

   >[!NOTE]
   >
   >Der Filter Gesendetes Datum basiert auf dem ersten Datum, an dem die E-Mail gesendet wurde.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Klicken Sie auf den Namen einer E-Mail, um sie in der E-Mail-Vorschau zu öffnen.

   >[!NOTE]
   >
   >Ein E-Mail-Leistungsbericht enthält Aktivitäten für alle Personen, einschließlich der Personen, die seit dem Versand der E-Mail gelöscht wurden. Manchmal möchten Sie Aktivitäten nur für aktive Personen sehen. In diesem Fall müssen Sie gelöschte Personen aus Ihrem Bericht herausfiltern. Verwenden Sie die **Smart List** Registerkarte zu [Erstellen von Smart-Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) für den Bericht. Wenn Sie nicht nach einem bestimmten Feld filtern, setzen Sie den Filter E-Mail-Adresse auf: **ist nicht leer**.

   [Berichtspalten auswählen](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) für einen E-Mail-Leistungsbericht:

   | Spalte | Beschreibung |
   |---|---|
   | Hard Bounce-Ereignis aufgetreten | E-Mail wurde wegen einer permanenten Bedingung wie einer nicht vorhandenen E-Mail-Adresse abgelehnt. |
   | Soft Bounce-Ereignis aufgetreten | E-Mail wurde wegen einer temporären Bedingung wie einem Server ausgeschaltet oder einem vollständigen Posteingang abgelehnt. |
   | Ausstehend | Diese Zahl wird berechnet, indem die Anzahl der zugestellten, Bounce und Softbounce gesendeten E-Mails von der Gesamtzahl der gesendeten E-Mails abgezogen wird. |
   | Angeklickter Link | Anzahl der E-Mail-Empfänger, die auf einen Link in der E-Mail geklickt haben |
   | Abgemeldet | Anzahl der E-Mail-Empfänger, die auf die **Abmelden** in der E-Mail klicken und das Formular ausfüllen. |

   >[!NOTE]
   >
   >Abmelde-Links und E-Mail-Adressen, auf die in einer E-Mail geklickt wird, werden nicht unter Klicks auf Links im Bericht registriert.

Im Allgemeinen versuchen wir, diese Statistiken mit gesundem Menschenverstand aufzuzeichnen. Wenn beispielsweise jemand in einer E-Mail auf einen Link geklickt hat, hat er die E-Mail offensichtlich zuerst geöffnet. Wir befolgen diese spezifischen Regeln für den E-Mail-Leistungsbericht:

* **Regel 1**: Jeder E-Mail-Aktivitätsdatensatz ist auf einen der folgenden Werte eingestellt: _Zugestellt_, _Hardbounce_, _Softbounce_ oder _Ausstehend_.

* **Regel 2**: Wenn der E-Mail-Datensatz *Geöffnet*, wird er als *Zugestellt*.

* **Regel 3**: Wenn der E-Mail-Datensatz _Angeklickte E-Mail_ oder _Abgemeldet_, wird er als _Zugestellt_ und _Geöffnet_.

* **Artikel 4**: Wenn die E-Mail _Geöffnet_, werden Absprünge ignoriert. Wenn die E-Mail nicht geöffnet wurde, _Hardbounce_ Vorrang vor _Softbounce_ und _Zugestellt_.

>[!NOTE]
>
>Mehrere Sendungen derselben Kampagne an dieselbe Person werden nur einmal gezählt.

>[!MORELIKETHIS]
>
>* [Filtern von Assets in Campaign-E-Mail-Berichten](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Leistungsbericht von E-Mail-Links](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
