---
unique-page-id: 2360297
description: Marketo-Anmeldungen auf Basis von IP einschränken - Marketo-Dokumente - Produktdokumentation
title: Marketo-Anmeldungen auf IP-Basis beschränken
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Marketo-Anmeldungen auf IP-Basis beschränken {#restrict-marketo-logins-based-on-ip}

Sie können Benutzer anhand ihrer IP-Adressen am Zugriff auf Marketo hindern bzw. daran hindern. So geht es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Die Informationen in diesem Artikel gelten nur für direkte Anmeldungen bei login.marketo.com. Es ist derzeit nicht möglich, IP-Einschränkungen für Single Sign-on (SSO)-Anmeldungen zu erzwingen.

1. under **Admin** klicken **Anmeldeeinstellungen**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. Klicken **IP-Einschränkungen bearbeiten**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. Auswählen, ob Sie **Zulassen** oder **Block** bestimmte Adressen, geben Sie die Adresse(n) ein und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **Zulässige IP-Adressen**: Das Hinzufügen erlaubter IP-Adressen ist inklusiv. Sie enthält alle angegebenen IP-Adressen und schließt alle anderen aus.
   >* **IP-Adressen blockieren**: Verhindert, dass bestimmte IPs auf Marketo zugreifen.
   >* **IP-Einschränkungen deaktivieren**: Wenn Sie dies überprüfen, funktionieren alle/alle Einschränkungsregeln nicht mehr. Verwenden Sie dies zu Testzwecken.


   >[!NOTE]
   >
   >Sie können mehrere Einschränkungen hinzufügen, diese können jedoch nur &quot;ALLE&quot;oder &quot;ALLE blockiert&quot;sein. Sie können nicht mischen und passend erlaubt und blockiert.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Ihre Marketing-Daten sind jetzt sicherer als je zuvor!
