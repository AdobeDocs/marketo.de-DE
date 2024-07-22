---
description: Einrichten des benutzerdefinierten Domänentrackings - Marketo-Dokumente - Produktdokumentation
title: Einrichten des Trackings benutzerdefinierter Domänen
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Einrichten des Trackings benutzerdefinierter Domänen {#how-to-set-up-custom-domain-tracking}

Mit dem benutzerdefinierten Domain-Tracking kann Ihr Team Ihren eigenen Unternehmensnamen in allen verfolgbaren Links verwenden, die zu Ihren Verkaufs-E-Mails hinzugefügt werden. Nachdem Sie diese Einstellung eingerichtet haben, werden alle Links, die Sie in Ihrer E-Mail haben, als go.yourcompany.com angezeigt, sodass, wenn ein Benutzer den Mauszeiger über einen Link bewegt, go.yourcompany.com anstelle von go.toutapp.com gelesen wird.

Sie benötigen Hilfe von Ihrem IT-Team, um einen CNAME-Eintrag für Ihre Domäne einzurichten, der auf go.toutapp.com verweist. Dieser CNAME wird auf allen Ihren Tracking-Links angezeigt (z. B. go.yourcompany.com).

Nachdem Sie mit Ihrem IT-Team bestätigt haben, dass der CNAME ordnungsgemäß konfiguriert ist, können Sie ihn der Seite Benutzerdefiniertes Domänenverfolgung in Aktionen hinzufügen.

>[!NOTE]
>
>Wenn Ihr CNAME nicht ordnungsgemäß eingerichtet ist und Sie ihn als Ihre benutzerdefinierte Domäne in Aktionen aktivieren, kann er Tracking-Links und Pixel beschädigen.

## Benutzerdefinierte Domänenverfolgung aktivieren {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen.**

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Tracking**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Geben Sie auf der Registerkarte &quot;Verfolgung benutzerdefinierter Domänen&quot;Ihren CNAME ein und klicken Sie auf **Verbinden**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
