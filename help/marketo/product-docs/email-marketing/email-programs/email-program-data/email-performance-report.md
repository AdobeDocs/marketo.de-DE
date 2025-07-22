---
unique-page-id: 2359467
description: E-Mail-Leistungsbericht - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Leistungsbericht
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 3%

---

# E-Mail-Leistungsbericht {#email-performance-report}

Erstellen Sie einen E-Mail-Leistungsbericht, um zu sehen, wie gut Ihre E-Mails mit Statistiken wie zugestellt, geöffnet, angeklickt usw. funktionieren.

1. [Erstellen Sie einen Bericht in einem Programm](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) und wählen Sie den **[!UICONTROL E-Mail]** Leistungs[Berichtstyp](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändern Sie den Berichtszeitrahmen](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) und klicken Sie auf die Registerkarte **[!UICONTROL Bericht]**.
1. Du bist da! Erkunden Sie nun den Bericht, um zu sehen, wie Ihre E-Mail(s) ausgeführt wurden.

   >[!NOTE]
   >
   >Der Filter Gesendet am basiert auf dem ersten Datum, an dem die E-Mail gesendet wurde.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Klicken Sie auf den Namen einer E-Mail, um sie in der E-Mail-Vorschau zu öffnen.

   >[!NOTE]
   >
   >Ein E-Mail-Leistungsbericht enthält Aktivitäten für alle Personen, einschließlich der Aktivitäten, die seit dem Versand der E-Mail gelöscht wurden. Manchmal möchten Sie Aktivitäten nur für aktive Personen sehen. In diesem Fall müssen Sie gelöschte Personen aus Ihrem Bericht filtern. Verwenden Sie die **[!UICONTROL Smart-Liste]**, um [eine Smart-Liste zu erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) für den Bericht. Wenn Sie nach keinem bestimmten Feld filtern, legen Sie für den Filter E-Mail-Adresse folgenden Wert fest: **[!UICONTROL ist nicht leer]**.

   [Berichtsspalten auswählen](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) für einen E-Mail-Leistungsbericht Folgendes enthalten:

   <table><thead>
<tr>
    <th>Spalte</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Hard Bounce-Ereignis aufgetreten</td>
    <td>E-Mail wurde aufgrund einer permanenten Bedingung, z. B. einer nicht vorhandenen E-Mail-Adresse, abgelehnt.</td>
  </tr>
  <tr>
    <td>Soft Bounce-Ereignis aufgetreten</td>
    <td>E-Mail wurde aufgrund einer temporären Bedingung abgelehnt, z. B. weil ein Server ausgefallen ist oder weil der Posteingang voll ist.</td>
  </tr>
  <tr>
    <td>Ausstehend</td>
    <td>Diese Zahl wird berechnet, indem von der Gesamtzahl der gesendeten E-Mails die Anzahl der zugestellten, gebouncten und Softbounces abgezogen wird.</td>
  </tr>
  <tr>
    <td>Angeklickter Link</td>
    <td>Die Anzahl der E-Mail-Empfänger, die auf einen Link in der E-Mail geklickt haben.</td>
  </tr>
  <tr>
    <td>Abbestellt</td>
    <td>Die Anzahl der E-Mail-Empfänger, die auf den Abmelde-Link in der E-Mail geklickt und das Formular ausgefüllt haben.</td>
  </tr>
  <tr>
    <td>Abgebrochen</td>
    <td>Anzahl der E-Mails, die nicht zugestellt werden konnten und kein Bounce-Ereignis empfangen wurde. Eine E-Mail wird automatisch als Abgebrochen bezeichnet, wenn nicht innerhalb von drei Tagen nach dem E-Mail-Versand eine Antwort empfangen wird.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Abmelde-Links und E-Mail-Adressen, die in einer E-Mail angeklickt werden, werden nicht unter angeklickten Links im Bericht registriert.

Im Allgemeinen versuchen wir, den gesunden Menschenverstand zu verwenden, um diese Statistiken aufzuzeichnen. Wenn beispielsweise jemand auf einen Link in einer E-Mail geklickt hat, hat er offensichtlich zuerst die E-Mail geöffnet. Für den E-Mail-Leistungsbericht befolgen wir diese spezifischen Regeln:

* **Regel 1**: Jeder E-Mail-Aktivitätsdatensatz ist auf einen und nur einen der folgenden Datensätze festgelegt: _Zugestellt_, _Hardbounce_, _Softbounce_ oder _Ausstehend_.

* **Regel 2**: Wenn der E-Mail-Datensatz *[!UICONTROL Geöffnet]* anzeigt, wird er als &quot;*&quot;*.

* **Regel 3**: Wenn der E-Mail-Datensatz _[!UICONTROL geklickte E-Mail]_ oder _[!UICONTROL Abgemeldet]_ anzeigt, wird er als _Zugestellt_ und _Geöffnet_ gezählt.

* **Regel 4**: Wenn die E-Mail _[!UICONTROL geöffnet]_ ist, werden Bounces ignoriert. Wenn die E-Mail nicht geöffnet wurde, hat _Hardbounce_ Vorrang vor _Softbounce_ und _Zugestellt_.

* **Regel 5**: Wenn drei Tage nach dem Versand keine E-Mail-Aktivität empfangen wird, gilt sie als _Abgebrochen_.

>[!NOTE]
>
>* Mehrere Sendungen von derselben Kampagne an dieselbe Person werden nur einmal gezählt.
>
>* Mehrere Sendungen von verschiedenen Kampagnen an dieselbe Person werden separat gezählt.

>[!MORELIKETHIS]
>
>* [Filtern von Assets in E-Mail-Berichten in Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtern Sie gelöschte/zusammengeführte Datensätze in einem E-Mail-Leistungsbericht](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Email Link Performance Report](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
