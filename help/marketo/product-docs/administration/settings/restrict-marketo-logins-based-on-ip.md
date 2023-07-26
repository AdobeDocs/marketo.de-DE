---
unique-page-id: 2360297
description: Marketo-Anmeldungen auf Basis von IP einschränken - Marketo-Dokumente - Produktdokumentation
title: Marketo-Anmeldungen auf IP-Basis beschränken
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Marketo-Anmeldungen auf IP-Basis beschränken {#restrict-marketo-logins-based-on-ip}

Sie können Benutzer anhand ihrer IP-Adressen am Zugriff auf Marketo hindern bzw. daran hindern. So geht es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Die Informationen in diesem Artikel gelten nur für direkte Anmeldungen unter login.marketo.com. Es ist derzeit nicht möglich, IP-Einschränkungen für Single Sign-on (SSO)-Anmeldungen zu erzwingen.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Klicks **[!UICONTROL Anmeldeeinstellungen]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Klicks **[!UICONTROL IP-Einschränkungen bearbeiten]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Auswählen, ob Sie **Zulassen** oder **Block** bestimmte Adressen, geben Sie die Adresse(n) ein und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **[!UICONTROL Zulässige IP-Adressen]**: Das Hinzufügen erlaubter IP-Adressen ist inklusiv. Sie enthält alle angegebenen IP-Adressen und schließt alle anderen aus.
   >* **[!UICONTROL IP-Adressen blockieren]**: Verhindert, dass bestimmte IPs auf Marketo zugreifen.
   >* **[!UICONTROL IP-Einschränkungen deaktivieren]**: Wenn Sie dies aktivieren, funktionieren alle/alle Einschränkungsregeln nicht mehr. Verwenden Sie dies zu Testzwecken.

   >[!NOTE]
   >
   >Sie können mehrere Einschränkungen hinzufügen, diese können jedoch nur &quot;ALLE&quot;oder &quot;ALLE blockiert&quot;sein. Sie können nicht mischen und passend erlaubt und blockiert.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Ihre Marketing-Daten sind jetzt sicherer als je zuvor!
