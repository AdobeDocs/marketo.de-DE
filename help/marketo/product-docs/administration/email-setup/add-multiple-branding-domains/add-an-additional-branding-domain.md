---
unique-page-id: 11377395
description: Fügen Sie zusätzliche Branding-Domains für mehrere Marken in einer Instanz hinzu, sodass jede über eigene Marken-Tracking-Links verfügt.
title: Hinzufügen einer zusätzlichen Branding-Domain
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 20%

---

# Hinzufügen einer zusätzlichen Branding-Domain {#add-an-additional-branding-domain}

Fügen Sie eine zusätzliche Branding-Domain hinzu, wenn Sie mehrere Marken von einer Marketo-Instanz aus ausführen und möchten, dass diese jeweils über eigene Branding-Tracking-Links verfügen.

>[!PREREQUISITES]
>
>Sie müssen [ generischen Tracking-Link durch ](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} Markendomäne ersetzen, bevor Sie weitere Markendomänen hinzufügen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Klicken Sie **[!UICONTROL Hinzufügen]**, um eine zusätzliche Branding-Domain hinzuzufügen.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Geben Sie den Namen Ihrer neuen Branding-Domain ein, wählen Sie _Primäre Domain erstellen_ und/oder _SSL-Zertifikat generieren_ (beide optional) aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Primäre Domain festlegen_: Wählen Sie diese als primäre Domain aus und alle vorhandenen nicht gesendeten E-Mails, die auf „Standard“ eingestellt sind, und alle neu erstellten E-Mails werden standardmäßig auf die primäre Domain festgelegt. Sie können [dies pro E-Mail überschreiben](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _SSL-Zertifikat generieren_: Sie können bei der Erstellung der Domain ein SSL (Secure Sockets Layer) erstellen. Die erste Tracking-Domain initiiert eine einmalige Einrichtung der Infrastruktur, die einige Stunden dauern kann. Sie werden nach Abschluss benachrichtigt, und Sie können dann die erste Domain einrichten. Um SSL zu Ihren bestehenden Domains hinzuzufügen, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}.

## SSLs für bestehende Domains bearbeiten

Führen Sie diese Schritte aus, um SSL für Ihre bestehenden Domains zu aktivieren.

1. Wählen Sie im Bereich _[!UICONTROL Admin]_ die Option **[!UICONTROL E-Mail]** aus.

1. Wählen Sie auf der Registerkarte _[!UICONTROL Domain]_ die Zeile Domain aus und klicken Sie auf **[!UICONTROL SSL hinzufügen]**.

   ![Admin - Email - Domain - SSL hinzufügen](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. Klicken Sie im Dialogfeld auf &quot;**[!UICONTROL &quot;]**.

   ![SSL hinzufügen - Bestätigen](./assets/generate-ssl-cert-confirm.png){width="400"}

## Fehlermeldungen {#error-messages}

<table><thead>
  <tr>
    <th>Fehler</th>
    <th>Details</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>Domäne existiert bereits.</i></td>
    <td>Eine Domain mit demselben Namen ist bereits vorhanden.</td>
  </tr>
  <tr>
    <td><i>Domain ist nicht der Standard-Domain zugeordnet.</i></td>
    <td>Die benutzerdefinierte Domain wird nicht korrekt der Standard-Domain zugeordnet. Überprüfen Sie die Einstellungen der Domain-Zuordnung und stellen Sie sicher, dass die DNS-Konfiguration auf die richtige Standard-Domain verweist.</td>
  </tr>
  <tr>
    <td><i>SSL-Zertifikate konnten aufgrund nicht unterstützter CAA-Einträge nicht ausgestellt werden. Fordern Sie Ihre IT an, Ihre CAA-Einträge zu aktualisieren.</i></td>
    <td>Die CAA-Einträge sind nicht aktuell. Für Benutzer, die von Marketo Engage verwaltete SSL-Zertifikate verwenden, müssen CAA-Einträge auf Zertifikate aktualisiert werden, die vom Marketo-Anbieter empfohlen werden. Wenden Sie sich an Ihre IT-Abteilung, um die CAA-Einträge zu aktualisieren. Weitere Informationen finden <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246"> auf </a> Seite .</td>
  </tr>
  <tr>
    <td><i>SSL-Zertifikat wurde bereits ausgestellt.</i></td>
    <td>Für diese benutzerdefinierte Domain ist bereits ein SSL-Zertifikat vorhanden. Es sind keine weiteren Maßnahmen erforderlich, es sei denn, das Zertifikat ist abgelaufen oder muss erneut ausgestellt werden.</td>
  </tr>
  <tr>
    <td><i>Die Standard-Domain wurde nicht gefunden. Bitte wenden Sie sich an den Support, um Hilfe zu erhalten.</i></td>
    <td>Beim Suchen der Standard-Domain ist ein Problem aufgetreten. Support kontaktieren, um eine Untersuchung durchzuführen.</td>
  </tr>
  <tr>
    <td><i>Unerwarteter Fehler beim Erstellen einer Domain. Bitte wenden Sie sich an den Support, um Hilfe zu erhalten.</i></td>
    <td>Ein unerwarteter Fehler ist aufgetreten. Sammeln Sie Protokolle und Fehlerdetails und eskalieren Sie das Problem an den <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo-Support</a>.</td>
  </tr>
</tbody></table>

## Zu beachtende Punkte {#things-to-note}

* **DNS-Zuordnung für Domain zu Marketo Engage**: Bevor Sie Domains in der Benutzeroberfläche hinzufügen, müssen Sie [CNAMEs einer von Marketo bereitgestellten Domain zuordnen](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Benutzerdefinierte SSL**: Wenn Sie eine benutzerdefinierte SSL benötigen, senden Sie ein [Support-Ticket](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}. Verwenden Sie nicht das Kontrollkästchen „Self-Service“ für die SSL-Erstellung.

* **Vorhandene SSLs**: Beim Hinzufügen einer Domain sucht das System nach bereits vorhandenen SSLs, die möglicherweise zuvor manuell erstellt wurden. Wenn diese Validierung auftritt, erstellen Sie Ihre Domain, ohne die SSL-Erstellung auszuwählen, und wenden Sie sich an [Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}, um sie verbinden zu lassen.

* **Löschen von Domains**: Beim automatischen Löschen einer Domain **das SSL** Zertifikat nicht gelöscht. Diese Schutzmaßnahme verhindert Benutzerfehler, die dazu führen, dass eine Website ohne SSL-Zertifikate ist. Wenn Sie die SSL-Zertifikate entfernen möchten, wenden Sie sich [ den Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}.

* Wenn die von Ihnen hinzugefügte Domain nicht als CNAME aufgeführt ist, wird die Möglichkeit zum Hinzufügen weiterer Marken-Tracking-Domains ausgeschlossen. Sie müssen eine vorhandene Domain bearbeiten und sicherstellen, dass es sich um einen CNAME-Eintrag und nicht beispielsweise um einen A-Eintrag handelt. Mit der Schaltfläche Hinzufügen wird nur dynamisch nach CNAME gesucht.

>[!MORELIKETHIS]
>
>[Standard-Branding-Domain bearbeiten](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
