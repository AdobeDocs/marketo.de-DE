---
unique-page-id: 2359467
description: E-Mail-Leistungsbericht - Marketing-Dokumente - Produktdokumentation
title: Bericht zur E-Mail-Leistung
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---


# E-Mail-Leistungsbericht {#email-performance-report}

Um zu sehen, wie gut Ihre E-Mails mit Statistiken wie Auslieferung, Öffnen, Klicken usw. funktionieren, erstellen Sie einen E-Mail-Leistungsbericht.

1. [Erstellen Sie einen Bericht in einem ](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) Programm und wählen Sie den  **Berichtstyp** [E-Mail-Leistung](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändern Sie den ](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) Berichtszeitrahmen und klicken Sie auf die Registerkarte  **** Bericht.
1. Du bist da! Sehen Sie sich den Bericht an, um zu sehen, wie Ihre E-Mail-Adresse(n) funktioniert hat.

   >[!NOTE]
   >
   >Der Filter &quot;Datum gesendet&quot;basiert auf dem ersten Datum, an dem die E-Mail gesendet wurde.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Klicken Sie auf den Namen einer E-Mail, um sie in der E-Mail-Vorschau zu öffnen.

   >[!NOTE]
   >
   >Ein E-Mail-Leistungsbericht enthält Aktivitäten für alle Personen, einschließlich derer, die seit dem Senden der E-Mail gelöscht wurden. Manchmal möchten Sie Aktivitäten nur für aktive Menschen sehen. In diesem Fall müssen Sie gelöschte Personen aus Ihrem Bericht filtern. Verwenden Sie die Registerkarte **Intelligente Liste**, um [eine intelligente Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) für den Bericht zu erstellen. Wenn Sie nicht nach einem bestimmten Feld filtern, setzen Sie den Filter E-Mail-Adresse auf: **ist nicht leer**.

   [Wählen Sie Berichtsspalten ](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) für einen E-Mail-Leistungsbericht aus:

   | Spalte | Beschreibung |
   |---|---|
   | Harter Absprung | Die E-Mail wurde aufgrund einer dauerhaften Bedingung wie z. B. einer nicht vorhandenen E-Mail-Adresse abgelehnt. |
   | Weich gebohrt | Die E-Mail wurde aufgrund einer temporären Bedingung wie dem Herunterfahren eines Servers oder einem vollständigen Posteingang abgelehnt. |
   | Ausstehend | Diese Zahl wird berechnet, indem die Anzahl der gesendeten E-Mails, Bounced und Soft Bounced von der Gesamtzahl der gesendeten E-Mails abgezogen wird. |
   | Klicken auf Link | Anzahl der E-Mail-Empfänger, die auf einen Link in der E-Mail geklickt haben. |
   | Nicht abonniert | Anzahl der E-Mail-Empfänger, die auf den Link **Abmelden** in der E-Mail geklickt und das Formular ausgefüllt haben. |

   >[!NOTE]
   >
   >Abmelden von Links und E-Mail-Adressen, auf die in einer E-Mail geklickt wird, werden nicht unter Klicks auf Links im Bericht registriert.

Im Allgemeinen versuchen wir, diese Statistiken mit dem gesunden Menschenverstand aufzuzeichnen. Wenn beispielsweise jemand in einer E-Mail auf einen Link geklickt hat, hat er die E-Mail offensichtlich zuerst geöffnet. Für den Bericht &quot;E-Mail-Leistung&quot;gelten die folgenden spezifischen Regeln:

* **Regel 1**: Jeder E-Mail-Aktivität-Datensatz ist auf einen der folgenden Werte eingestellt:  _Ausgeliefert_,  _harter Absprung_,  _weich abgeschnitten_ oder  _ausstehend_.

* **Regel 2**: Wenn der E-Mail-Datensatz &quot; *Geöffnet*&quot;anzeigt, wird er als  *&quot;Ausgeliefert*&quot;gezählt.

* **Artikel 3**: Wenn der E-Mail-Datensatz  _Klicks auf_ E-Mail-Adresse  _abbestellt_ anzeigt, wird er als  __ Ausgeliefert und  _geöffnet_ gezählt.

* **Artikel 4**: Wenn die E-Mail  _geöffnet_ ist, werden Absprünge ignoriert. Wenn die E-Mail nicht geöffnet wurde, hat _Hard Bounced_ Vorrang vor _Soft Bounced_ und _Delivered_.

>[!NOTE]
>
>Mehrere Sends von derselben Kampagne an dieselbe Person werden nur einmal gezählt.

>[!MORELIKETHIS]
>
>* [Assets in Kampagne-E-Mail-Berichten filtern](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Leistungsbericht zu E-Mail-Links](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

