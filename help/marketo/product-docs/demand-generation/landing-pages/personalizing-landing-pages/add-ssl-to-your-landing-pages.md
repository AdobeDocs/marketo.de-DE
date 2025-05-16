---
unique-page-id: 2359828
description: Hinzufügen von SSL zu Ihren Landingpages - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von SSL zu Ihren Landingpages
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Hinzufügen von SSL zu Ihren Landingpages {#add-ssl-to-your-landing-pages}

Mit der SSL-Verschlüsselung (Secure Socket Layer) können Sie alle Landingpages für eine Marketo Engage-Instanz sicher machen.

Wenn Sie ein Web-Formular ausfüllen oder eine Landingpage besuchen, die von Marketo Engage gehostet wird, werden die Informationen standardmäßig über ein nicht sicheres Protokoll (HTTP) gesendet. Gemäß der Richtlinie Ihres Unternehmens möchten Sie möglicherweise die an Marketo gesendeten Informationen über (HTTPS) sichern. Wenn Sie beispielsweise `http://info.mydomain.com/` besuchen, wird es jetzt `https://info.mydomain.com/`.

Marketo Engage verfolgt „Besuchte Web-Seite“ und „Link auf Web-Seite klicken“ standardmäßig über das nicht sichere HTTP-Protokoll. Wenn Sie möchten, dass Ihre Tracking-Links mit einem eigenen Zertifikat gesichert werden, müssen Sie Marketo einen separaten, nicht freigegebenen Server erstellen lassen, um ihn zu aktivieren. Um alle Aspekte der Interaktion eines Kontakts mit Ihnen zu sichern, müssen in der Regel sowohl Landingpages als auch Tracking-Links gesichert werden.

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
>* Die Spalte SSL-Zertifikat in der Liste zeigt den Zertifikatstatus für den gesamten Domain-Alias an, der nach der Veröffentlichung dieser Funktion erstellt wurde (DATUM). Wenn Sie SSL für eine Domain über den Marketo-Support aktiviert haben, ist das Zertifikat weiterhin vorhanden, wird aber nicht in der Tabelle angezeigt. Diese Tabelle enthält nur SSL-Zertifikate für Domains, die mithilfe der Schritte in diesem Artikel hinzugefügt wurden.
>
>* Es kann bis zu drei Minuten dauern, bis SSL BEREIT ist. Sie müssen die Seite aktualisieren, damit die Änderungen angezeigt werden.
