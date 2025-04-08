---
description: Hinzufügen von SSL zu Ihren Landingpages - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von SSL zu Ihren Landingpages
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Hinzufügen von SSL zu Ihren Landingpages {#add-ssl-to-your-landing-pages}

Erfahren Sie, wie Sie den Alias Ihrer Marken-Domain (z. B. `http://business.adobe.com`) zu in Marketo Engage erstellten Landingpages hinzufügen, damit der Zugriff unter den jeweiligen Marken-Domains möglich ist.

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

## SSL für Standard-Domain aktivieren

SCREENSHOT

>[!NOTE]
>
>* Die Spalte SSL-Zertifikat in der Liste zeigt den Zertifikatstatus für den gesamten Domain-Alias an, der nach der Veröffentlichung dieser Funktion erstellt wurde (DATUM). Wenn Sie SSL für eine Domain über den Marketo-Support aktiviert haben, ist das Zertifikat weiterhin vorhanden, wird aber nicht in der Tabelle angezeigt. Diese Tabelle enthält nur SSL-Zertifikate für Domains, die mithilfe der Schritte in diesem Artikel hinzugefügt wurden.
>
>* Es kann bis zu drei Minuten dauern, bis SSL BEREIT ist. Sie müssen die Seite aktualisieren, damit die Änderungen angezeigt werden.
