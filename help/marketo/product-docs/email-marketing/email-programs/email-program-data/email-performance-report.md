---
unique-page-id: 2359467
description: E-Mail-Leistungsbericht - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Leistungsbericht
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 6133a04124d9d4b829d092943753c7bb530dd374
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 3%

---

# E-Mail-Leistungsbericht {#email-performance-report}

Erstellen Sie einen E-Mail-Leistungsbericht, um zu sehen, wie gut Ihre E-Mails mit Statistiken wie Zugestellt, Öffnungen, Klicks usw. funktionieren.

1. [Erstellen Sie einen Bericht in einem Programm](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) und wählen Sie den Berichtstyp **E-Mail-Leistung** [ ](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md) aus.
1. [Ändern Sie den Berichtszeitrahmen](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) und klicken Sie auf die Registerkarte **Bericht** .
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
   >Ein E-Mail-Leistungsbericht enthält Aktivitäten für alle Personen, einschließlich der Personen, die seit dem Versand der E-Mail gelöscht wurden. Manchmal möchten Sie Aktivitäten nur für aktive Personen sehen. In diesem Fall müssen Sie gelöschte Personen aus Ihrem Bericht herausfiltern. Verwenden Sie die Registerkarte **Smart-Liste** , um [eine Smart-Liste zu erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) für den Bericht. Wenn Sie nicht nach einem bestimmten Feld filtern, setzen Sie den Filter E-Mail-Adresse auf: **ist nicht leer**.

   [Berichtspalten auswählen](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) für einen E-Mail-Leistungsbericht:

   <table><thead>
<tr>
    <th>Spalte</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Hard Bounce-Ereignis aufgetreten</td>
    <td>E-Mail wurde wegen einer permanenten Bedingung wie einer nicht vorhandenen E-Mail-Adresse abgelehnt.</td>
  </tr>
  <tr>
    <td>Soft Bounce-Ereignis aufgetreten</td>
    <td>E-Mail wurde wegen einer temporären Bedingung wie einem Server ausgeschaltet oder einem vollständigen Posteingang abgelehnt.</td>
  </tr>
  <tr>
    <td>Ausstehend</td>
    <td>Diese Zahl wird berechnet, indem die Anzahl der zugestellten, Bounce und Softbounce gesendeten E-Mails von der Gesamtzahl der gesendeten E-Mails abgezogen wird.</td>
  </tr>
  <tr>
    <td>Angeklickter Link</td>
    <td>Anzahl der E-Mail-Empfänger, die auf einen Link in der E-Mail geklickt haben</td>
  </tr>
  <tr>
    <td>Abbestellt</td>
    <td>Anzahl der E-Mail-Empfänger, die auf den Link Abmelden in der E-Mail geklickt und das Formular ausgefüllt haben.</td>
  </tr>
  <tr>
    <td>Abgebrochen</td>
    <td>Anzahl der E-Mails, die nicht zugestellt werden konnten und kein Bounce-Ereignis empfangen wurde. Eine E-Mail wird automatisch als Abgebrochen bezeichnet, wenn innerhalb von drei Tagen nach dem Versand der E-Mail keine Antwort eingeht.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Abmelde-Links und E-Mail-Adressen, auf die in einer E-Mail geklickt wird, werden nicht unter Klicks auf Links im Bericht registriert.

Im Allgemeinen versuchen wir, diese Statistiken mit gesundem Menschenverstand aufzuzeichnen. Wenn beispielsweise jemand in einer E-Mail auf einen Link geklickt hat, hat er die E-Mail offensichtlich zuerst geöffnet. Wir befolgen diese spezifischen Regeln für den E-Mail-Leistungsbericht:

* **Regel 1**: Jeder E-Mail-Aktivitätsdatensatz ist auf einen der folgenden Werte festgelegt: _Zugestellt_, _Hard Bounce_, _Softbounce_ oder _Ausstehend_.

* **Regel 2**: Wenn der E-Mail-Datensatz den Wert *Geöffnet* aufweist, wird er als *Zugestellt* gezählt.

* **Regel 3**: Wenn der E-Mail-Datensatz _angeklickte E-Mail_ oder _abgemeldet_ anzeigt, wird er als _Zugestellt_ und _Geöffnet_ gezählt.

* **Regel 4**: Wenn die E-Mail _geöffnet_ ist, werden Bounces ignoriert. Wenn die E-Mail nicht geöffnet wurde, hat _Hard Bounce_ Vorrang vor _Soft Bounce_ und _Delivered_.

* **Regel 5**: Wenn drei Tage nach dem Versand keine E-Mail-Aktivität empfangen wird, gilt dies als _Abgebrochen_.

>[!NOTE]
>
>* Mehrere Sendungen derselben Kampagne an dieselbe Person werden nur einmal gezählt.
>
>* Mehrere Sendungen aus verschiedenen Kampagnen an dieselbe Person werden separat gezählt.

>[!MORELIKETHIS]
>
>* [Filtern von Assets in Campaign-E-Mail-Berichten](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Gelöschte/zusammengeführte Datensätze in einem E-Mail-Leistungsbericht filtern](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Leistungsbericht von E-Mail-Links](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
