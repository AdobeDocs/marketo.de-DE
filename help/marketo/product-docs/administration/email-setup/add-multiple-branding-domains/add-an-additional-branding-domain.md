---
unique-page-id: 11377395
description: Hinzufügen einer zusätzlichen Branding-Domain - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen einer zusätzlichen Branding-Domain
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: dafac137a6c626794f3b9b2bfaa2fc2de9f2cb75
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 3%

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

   ![](assets/add-an-additional-branding-domain-3.png)

1. Geben Sie den Namen Ihrer neuen Branding-Domain ein, wählen Sie _Primäre Domain erstellen_ und/oder _SSL-Zertifikat generieren_ (beide optional) aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Als Primäre Domain festlegen_: Als primäre Domain festlegen, wird für alle bestehenden nicht gesendeten E-Mails der Standardwert festgelegt und für alle neu erstellten E-Mails wird standardmäßig die primäre Domain verwendet. Sie können [dies pro E-Mail überschreiben](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _SSL-Zertifikat generieren_: Sie können bei der Erstellung der Domain ein SSL (Secure Sockets Layer) erstellen. Die erste Tracking-Domain initiiert eine einmalige Einrichtung der Infrastruktur, die einige Stunden dauern kann. Sie werden nach Abschluss benachrichtigt, und Sie können dann die erste Domain einrichten. Wenn Sie SSL zu Ihren bestehenden Domains hinzufügen möchten, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Fehlermeldungen {#error-messages}

<table><thead>
  <tr>
    <th>Fehler</th>
    <th>Details</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Unerwarteter Fehler beim Erstellen einer Domain. Bitte wenden Sie sich an den Support, um Hilfe zu erhalten.</i></td>
    <td>Ein unerwarteter Fehler ist aufgetreten. Bitte Protokolle und Fehlerdetails sammeln und das Problem an den <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo-Support</a> eskalieren.</td>
  </tr>
  <tr>
    <td><i>SSL-Zertifikat wurde bereits ausgestellt.</i></td>
    <td>Für diese benutzerdefinierte Domain ist bereits ein SSL-Zertifikat vorhanden. Es sind keine weiteren Maßnahmen erforderlich, es sei denn, das Zertifikat ist abgelaufen oder muss erneut ausgestellt werden.</td>
  </tr>
  <tr>
    <td><i>Domain ist nicht der Standard-Domain zugeordnet.</i></td>
    <td>Die benutzerdefinierte Domain wird nicht korrekt der Standard-Domain zugeordnet. Überprüfen Sie die Einstellungen der Domain-Zuordnung und stellen Sie sicher, dass die DNS-Konfiguration auf die richtige Standard-Domain verweist.</td>
  </tr>
  <tr>
    <td><i>Die Einrichtung von Cloudflare wurde initiiert. Bitte versuchen Sie es später erneut.</i></td>
    <td>Wenn Sie die erste Tracking-Domain für die Instanz erstellen, wird eine einmalige Infrastruktureinrichtung in Cloudfare durchgeführt. Diese Meldung zeigt an, dass die Einrichtung eingeleitet wurde und bis zu drei Stunden dauern kann.</td>
  </tr>
  <tr>
    <td><i>Die Cloudflare-Einrichtung ist noch in Bearbeitung. Bitte versuchen Sie es später erneut.</i></td>
    <td>Siehe oben</td>
  </tr>
  <tr>
    <td><i>Die Cloudflare-Einrichtung ist aufgrund eines unerwarteten Fehlers fehlgeschlagen. Wenden Sie sich an den Support.</i></td>
    <td>Die Einrichtung der Cloudfare-Infrastruktur ist fehlgeschlagen. Wenden Sie sich an den <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo-Support</a>, um Hilfe zu erhalten.</td>
  </tr>
</tbody></table>

## Zu beachtende Punkte {#things-to-note}

* **DNS-Zuordnung für Domain zu Marketo Engage**: Bevor Sie Domains in der Benutzeroberfläche hinzufügen, müssen Sie [CNAMEs einer von Marketo bereitgestellten Domain zuordnen](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Benutzerdefinierte SSLs**: Wenn Sie eine benutzerdefinierte SSL benötigen, senden Sie ein [Support-Ticket](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Verwenden Sie nicht das Kontrollkästchen „Self-Service“ für die SSL-Erstellung.

* **Vorhandene SSLs**: Beim Hinzufügen einer Domain sucht das System nach bereits vorhandenen SSLs, die möglicherweise zuvor manuell erstellt wurden. Wenn diese Validierung auftritt, erstellen Sie Ihre Domain, ohne die SSL-Erstellung auszuwählen, und wir werden sie für Sie verbinden. [Support kontaktieren](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} weitere Details/Optionen.

* **Domain für die Erstverfolgung**: Bei der erstmaligen Erstellung von Domains für E-Mail-Tracking-Links ist ein manuelles Eingreifen des [Marketo-Supports erforderlich](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Die nachfolgende Erstellung einer Subdomain unter derselben Domain ist in der Benutzeroberfläche zulässig.

* **Hinzufügen von Zertifikaten zu vorhandenen Domains**: Das Hinzufügen von Zertifikaten zu vorhandenen Domains wird derzeit nicht unterstützt. Für bereits bestehende Domains oder für Fälle, in denen Sie das Kontrollkästchen „SSL-Zertifikat“ nicht aktiviert haben, müssen Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} wenden, um das Zertifikat hinzuzufügen.

* **Bearbeiten oder Entfernen von Zertifikaten auf bestehenden Domains**: Wenn Sie eine vorhandene SSL aktualisieren oder entfernen müssen, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* **Löschen von Domains**: Beim Löschen einer Domain wird das SSL-Zertifikat derzeit nicht automatisch gelöscht. Dies wird in einer zukünftigen Version behoben.

>[!MORELIKETHIS]
>
>[Standard-Branding-Domain bearbeiten](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
