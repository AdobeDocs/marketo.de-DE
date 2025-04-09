---
description: Hinzufügen von SSL zu Ihren Landingpages - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von SSL zu Ihren Landingpages
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Hinzufügen von SSL zu Ihren Landingpages {#add-ssl-to-your-landing-pages}

Mit der SSL-Verschlüsselung (Secure Socket Layer) können Sie alle Landingpages für eine Marketo Engage-Instanz sicher machen.

Wenn Sie ein Web-Formular ausfüllen oder eine Landingpage besuchen, die von Marketo Engage gehostet wird, werden die Informationen standardmäßig über ein nicht sicheres Protokoll (HTTP) gesendet. Gemäß der Richtlinie Ihres Unternehmens möchten Sie möglicherweise die an Marketo gesendeten Informationen über (HTTPS) sichern. Wenn Sie beispielsweise `http://info.mydomain.com/` besuchen, wird es jetzt `https://info.mydomain.com/`.

Marketo Engage verfolgt „Besuchte Web-Seite“ und „Link auf Web-Seite klicken“ standardmäßig über das nicht sichere HTTP-Protokoll. Wenn Sie möchten, dass Ihre Tracking-Links mit einem eigenen Zertifikat gesichert werden, müssen Sie Marketo einen separaten, nicht freigegebenen Server erstellen lassen, um ihn zu aktivieren. Um alle Aspekte der Interaktion eines Kontakts mit Ihnen zu sichern, müssen in der Regel sowohl Landingpages als auch Tracking-Links gesichert werden.

SCREENSHOT

## SSL-Zertifizierung aktivieren {#enable-ssl-certification}

SSL automatisch für alle Domain-Aliase hinzufügen, die Sie im Rahmen der Landingpage-Regeln erstellen.

1. Navigieren Sie zum Bereich **Admin**.

   SCREENSHOT

1. Wählen Sie **Landingpages** aus der Baumstruktur aus. Klicken Sie auf **Registerkarte** Regeln **auf die Dropdown-Liste Neu** und wählen Sie **Neuer Domain-Alias**.

   SCREENSHOT

1. Aktivieren Sie das **SSL-Zertifikat generieren**.

   SCREENSHOT

Dadurch wird automatisch ein SSL-Zertifikat für diese Domain hinzugefügt.

SCREENSHOT

## SSL für Standard-Domain aktivieren {#enable-ssl-default-domain}

SCREENSHOT

>[!NOTE]
>
>* Die Spalte SSL-Zertifikat in der Liste zeigt den Zertifikatstatus für den gesamten Domain-Alias an, der nach der Veröffentlichung dieser Funktion erstellt wurde (DATUM). Wenn Sie SSL für eine Domain über den Marketo-Support aktiviert haben, ist das Zertifikat weiterhin vorhanden, wird aber nicht in der Tabelle angezeigt. Diese Tabelle enthält nur SSL-Zertifikate für Domains, die mithilfe der Schritte in diesem Artikel hinzugefügt wurden.
>
>* Es kann bis zu drei Minuten dauern, bis SSL BEREIT ist. Sie müssen die Seite aktualisieren, damit die Änderungen angezeigt werden.
