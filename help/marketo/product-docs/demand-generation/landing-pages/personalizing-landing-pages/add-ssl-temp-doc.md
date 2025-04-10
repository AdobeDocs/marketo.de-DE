---
description: hinzufügen SSL für Ihre Landing Seiten - Marketo Docs - Product Dokumentation
title: hinzufügen SSL für Ihre Seiten
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: c7bf6c7ffca16e95f13a7009897bce6fc39a9ffd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# hinzufügen SSL für Ihre Seiten {#add-ssl-to-your-landing-pages}

Mit SSL-Verschlüsselung (Secure Socket Ebene) können Sie alle Ihre Landing Seiten für ein Marketo Engage Instanz sicher machen.

Wenn Sie ein Webformular ausfüllen oder eine Landing-Seite Visit, die von Marketo Engage gehostet wird, werden die Informationen standardmäßig über ein nicht sicheres Protokoll (HTTP) gesendet. Gemäß den Regel Ihrer Firma können Sie die an Marketo übermittelten Informationen über (HTTPS) sichern. Wenn Sie z. B. Visit `http://info.mydomain.com/` , ist `https://info.mydomain.com/`es jetzt .

Marketo Engage verfolgt &quot;Besuchtes Web Seite&quot; und &quot;Klicken auf Link im Web Seite&quot; standardmäßig über ein nicht sicheres HTTP-Protokoll. Wenn Sie möchten, dass Ihre Tracking Links mit einem eigenen Zertifikat gesichert werden, müssen Sie Marketo einen separaten, nicht freigegebenen Server Build lassen, um ihn zu aktivieren. Um alle Aspekte der Interaktion eines Kontakts mit Ihnen zu sichern, müssen in der Regel sowohl Landing Seiten als auch Tracking Links gesichert werden.

## SSL-Zertifizierung aktivieren {#enable-ssl-certification}

Fügen Sie SSL automatisch für alle Domänenaliase hinzu, die Sie im Rahmen der Landing Seite Regeln erstellen.

1. OK in den **Admin-Bereich** .

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Wählen Sie in der Struktur die Option **&quot;Landing Seiten** &quot; aus. Klicken Sie im Tab Regel **auf das** Dropdown-Menü &quot;Neu **&quot; und wählen Sie &quot;Neu Domänenalias**&quot; aus **.**

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Geben Sie Ihren _Domain-Alias_ ein und _Standardmäßig Seite_. Aktivieren Sie das **Kontrollkästchen &quot;SSL-Zertifikat** generieren&quot;. Klicken Sie auf **Erstellen** , wenn Sie fertig sind.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Dadurch wird automatisch ein SSL-Zertifikat für diese Domäne hinzugefügt.

## Aktivieren von SSL für Ihre Standarddomäne {#enable-ssl-default-domain}

Gehen Sie wie folgt vor, um SSL für Ihre Standarddomäne zu aktivieren.

1. Wählen Sie im **Abschnitt &quot;Admin** &quot; die Option **&quot;Landing Seiten**&quot;. Klicken Sie auf das orangefarbene **Bearbeiten** Button neben _Einstellungen_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Falls gewünscht, können Sie hier auch den Domainnamen ändern (gültige Domain erforderlich).

1. Aktivieren Sie das Kontrollkästchen &quot;SSL-Zertifikat generieren&quot; und klicken Sie auf &quot;Speichern&quot;.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* Die Spalte &quot;SSL-Zertifikat&quot; in der Auflistung zeigt den Zertifikatsstatus für alle Domain-Alias, die nach der Veröffentlichung dieser Funktion erstellt wurden (DATE). Wenn Sie SSL für eine Domäne über den Marketo-Support aktiviert haben, ist das Zertifikat weiterhin vorhanden, wird jedoch nicht in der Tabelle angezeigt. Diese Tabelle enthält nur SSL-Zertifikate für Domänen, die mit den Schritten in diesem Artikel hinzugefügt wurden.
>
>* Es kann bis zu drei Minuten dauern, bis SSL den Status BEREIT aufweist. Sie müssen die Seite aktualisieren, damit die Änderungen übernommen werden.
