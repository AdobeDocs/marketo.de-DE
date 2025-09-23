---
unique-page-id: 2359828
description: Hinzufügen von SSL zu Ihren Landingpages - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von SSL zu einer Landingpage
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 2%

---

# Hinzufügen von SSL zu einer Landingpage {#add-ssl-to-your-landing-pages}

Mit der SSL-Verschlüsselung (Secure Socket Layer) können Sie alle Landingpages für eine Marketo Engage-Instanz sicher machen.

Wenn Sie ein Web-Formular ausfüllen oder eine Landingpage besuchen, die von Marketo Engage gehostet wird, werden die Informationen standardmäßig über ein nicht sicheres Protokoll (HTTP) gesendet. Gemäß der Richtlinie Ihres Unternehmens möchten Sie möglicherweise die an Marketo gesendeten Informationen über (HTTPS) sichern. Wenn Sie beispielsweise `http://info.mydomain.com/` besuchen, wird es jetzt `https://info.mydomain.com/`.

Marketo Engage verfolgt „Besuchte Web-Seite“ und „Link auf Web-Seite klicken“ standardmäßig über das nicht sichere HTTP-Protokoll. Wenn Sie möchten, dass Ihre Tracking-Links mit einem eigenen Zertifikat gesichert werden, müssen Sie Marketo einen separaten, nicht freigegebenen Server erstellen lassen, um ihn zu aktivieren. Um alle Aspekte der Interaktion eines Kontakts mit Ihnen zu sichern, müssen in der Regel sowohl Landingpages als auch Tracking-Links gesichert werden.

>[!IMPORTANT]
>
>Bevor Sie eine SSL hinzufügen, überprüfen Sie Ihren Vertrag auf die Gesamtzahl der Domains, die Sie hinzufügen dürfen. Andernfalls können Sie eine Gebühr entrichten. Wenn Sie die Informationen nicht finden können, wenden Sie sich bitte an das Adobe Account Team (Ihren Account Manager), um weitere Informationen zu erhalten.

## SSL-Zertifizierung aktivieren {#enable-ssl-certification}

SSL automatisch für alle Domain-Aliase hinzufügen, die Sie im Rahmen der Landingpage-Regeln erstellen.

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Wählen Sie **Landingpages** aus der Baumstruktur aus. Klicken Sie auf **Registerkarte** Regeln **auf die Dropdown-Liste Neu** und wählen Sie **Neuer Domain-Alias**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Geben Sie Ihren _Domain-_) und _Standardseite_ ein. Aktivieren Sie das **SSL-Zertifikat generieren**. Klicken Sie **Erstellen** wenn Sie fertig sind.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Dadurch wird automatisch ein SSL-Zertifikat für diese Domain hinzugefügt.

## SSL für Standard-Domain aktivieren {#enable-ssl-default-domain}

Gehen Sie wie folgt vor, um SSL für Ihre Standard-Domain zu aktivieren.

1. Wählen Sie noch im **Admin**-Bereich **Landingpages** aus. Klicken Sie auf die orangefarbene **Bearbeiten**-Schaltfläche neben _Einstellungen_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Bei Bedarf können Sie hier auch den Domain-Namen ändern (gültige Domain erforderlich).

1. Aktivieren Sie das Kontrollkästchen „SSL-Zertifikat generieren“ und klicken Sie auf Speichern.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>Es kann bis zu drei Minuten dauern, bis SSL den Status BEREIT aufweist. Seite aktualisieren, damit die Änderungen angezeigt werden.

## SSLs zu vorhandenen Domain-Aliassen bearbeiten

Führen Sie diese Schritte aus, um SSL für Ihre vorhandenen Domain-Aliase zu aktivieren.

1. Erweitern Sie im _[!UICONTROL Admin]_-Bereich **[!UICONTROL Integration]** im linken Navigationsbereich und wählen Sie **[!UICONTROL Landingpages]**.

1. Wählen Sie auf der Seite oben die **[!UICONTROL Regeln]** aus.

1. Wählen Sie die Domain-Alias-Zeile aus, die Sie bearbeiten möchten, und klicken Sie oben **[!UICONTROL SSL hinzufügen]**.

   ![Admin-Bereich - Integration > Landingpages - Registerkarte „Regeln“ - Domain-Alias auswählen](./assets/admin-landing-pages-rules-add-ssl.png){width="800" zoomable="yes"}

1. Klicken Sie im Dialogfeld auf &quot;**[!UICONTROL &quot;]**.

   ![SSL hinzufügen - Bestätigen](./assets/generate-ssl-cert-confirm.png){width="400"}

>[!NOTE]
>
>Es kann bis zu drei Minuten dauern, bis SSL den Status BEREIT aufweist. Seite aktualisieren, damit die Änderungen angezeigt werden.

## Fehlermeldungen {#error-messages}

Unten finden Sie Fehlermeldungen, die Sie möglicherweise zusammen mit ihren Definitionen erhalten.

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
    <td>Die CAA-Einträge sind nicht aktuell. Für Benutzer, die von Marketo Engage verwaltete SSL-Zertifikate verwenden, müssen CAA-Einträge auf Zertifikate aktualisiert werden, die von unserem Anbieter empfohlen werden. Bitte wenden Sie sich an Ihre IT-Abteilung, um die CAA-Einträge zu aktualisieren. Weitere Informationen finden <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246"> auf </a> Seite .</td>
  </tr>
  <tr>
    <td><i>SSL-Zertifikat wurde bereits ausgestellt.</i></td>
    <td>Für diese benutzerdefinierte Domain ist bereits ein SSL-Zertifikat vorhanden. Es sind keine weiteren Maßnahmen erforderlich, es sei denn, das Zertifikat ist abgelaufen oder muss erneut ausgestellt werden.</td>
  </tr>
  <tr>
    <td><i>Die Standard-Domain wurde nicht gefunden. Bitte wenden Sie sich an den Support, um Hilfe zu erhalten.</i></td>
    <td>Beim Suchen der Standard-Domain ist ein Problem aufgetreten. Bitte wenden Sie sich an den Support, damit er weitere Informationen erhalten kann.</td>
  </tr>
  <tr>
    <td><i>Unerwarteter Fehler beim Erstellen einer Domain. Bitte wenden Sie sich an den Support, um Hilfe zu erhalten.</i></td>
    <td>Ein unerwarteter Fehler ist aufgetreten. Bitte Protokolle und Fehlerdetails sammeln und das Problem an den <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo-Support</a> eskalieren.</td>
  </tr>
</tbody></table>

## Zu beachtende Punkte {#things-to-note}

* **DNS-Zuordnung für Domain zu Marketo Engage**: Bevor Sie Domains in der Benutzeroberfläche hinzufügen, müssen Sie [CNAMEs einer von Marketo bereitgestellten Domain zuordnen](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Benutzerdefinierte SSLs**: Wenn Sie eine benutzerdefinierte SSL benötigen, senden Sie ein [Support-Ticket](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Verwenden Sie nicht das Kontrollkästchen „Self-Service“ für die SSL-Erstellung.

* **Vorhandene SSLs**: Beim Hinzufügen einer Domain sucht das System nach bereits vorhandenen SSLs, die möglicherweise zuvor manuell erstellt wurden. Wenn diese Validierung auftritt, erstellen Sie Ihre Domain, ohne die SSL-Erstellung auszuwählen, und wir werden sie für Sie verbinden. [Support kontaktieren](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} weitere Details/Optionen.

* **Löschen von Domains**: Beim automatischen Löschen einer Domain **das SSL** Zertifikat nicht gelöscht. Diese Schutzmaßnahme verhindert Benutzerfehler, die dazu führen, dass eine Website ohne SSL-Zertifikate ist. Wenn Sie die SSL-Zertifikate entfernen möchten, wenden Sie sich [ den Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
