---
unique-page-id: 2360297
description: Marketo-Anmeldungen auf Basis von IP beschränken - Marketo-Dokumente - Produktdokumentation
title: Beschränken von Marketo-Anmeldungen auf der Grundlage von IP-Adressen
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b4bd06d3e5ee205744478e0f5556f490f9f5abe4
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Beschränken von Marketo-Anmeldungen auf der Grundlage von IP-Adressen {#restrict-marketo-logins-based-on-ip}

Sie können den Zugriff von Benutzenden auf Marketo anhand ihrer IP-Adressen einschränken oder aktivieren. So geht&#39;s.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel richten sich an Benutzer, die sich direkt unter login.marketo.com anmelden. Sie gelten nicht für Benutzer, die sich bei Adobe ID authentifizieren. Es ist derzeit nicht möglich, IP-Einschränkungen für SSO-Anmeldungen (Single Sign-on) durchzusetzen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Klicken Sie **[!UICONTROL Anmeldeeinstellungen]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Klicken Sie **[!UICONTROL IP-Einschränkungen bearbeiten]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Wählen Sie aus, ob **Adressen zugelassen** **blockiert** sollen, geben Sie die Adresse(n) ein und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **[!UICONTROL Zulässige IP-Adressen]**: Das Hinzufügen zulässiger IP-Adressen erfolgt inklusiv. Es enthält alle angegebenen IP-Adressen und schließt alles andere aus.
   >* **[!UICONTROL IP-Adressen blockieren]**: Verhindert den Zugriff bestimmter IPs auf Marketo.
   >* **[!UICONTROL IP-Einschränkungen deaktivieren]**: Wenn Sie diese Option aktivieren, funktionieren keine/alle Einschränkungsregeln mehr. Verwenden Sie dies zu Testzwecken.

   >[!NOTE]
   >
   >Sie können mehrere Einschränkungen hinzufügen, sie können jedoch nur ALLE zulässig oder ALLE blockiert sein. Zulässig und blockiert können nicht gemischt und übereinstimmen.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Gut gemacht, Ihre Marketing-Daten sind jetzt sicherer als je zuvor!
