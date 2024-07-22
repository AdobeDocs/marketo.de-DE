---
unique-page-id: 2360297
description: Marketo-Anmeldungen auf Basis von IP einschränken - Marketo-Dokumente - Produktdokumentation
title: Marketo-Anmeldungen auf IP-Basis beschränken
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b4bd06d3e5ee205744478e0f5556f490f9f5abe4
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Marketo-Anmeldungen auf IP-Basis beschränken {#restrict-marketo-logins-based-on-ip}

Sie können Benutzer anhand ihrer IP-Adressen am Zugriff auf Marketo hindern bzw. daran hindern. So geht es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel richten sich an Benutzer, die sich direkt unter login.marketo.com anmelden, und gelten nicht für Benutzer, die sich bei Adobe ID authentifizieren. Derzeit ist es nicht möglich, IP-Einschränkungen für Single Sign-on (SSO)-Anmeldungen zu erzwingen.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Klicken Sie auf **[!UICONTROL Anmeldeeinstellungen]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Klicken Sie auf **[!UICONTROL IP-Einschränkungen bearbeiten]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Wählen Sie aus, ob Sie bestimmte Adressen **Zulassen** oder **Blockieren** verwenden möchten, geben Sie die Adressen ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **[!UICONTROL Zulässige IP-Adressen]**: Das Hinzufügen erlaubter IP-Adressen ist inklusiv. Sie enthält alle angegebenen IP-Adressen und schließt alle anderen aus.
   >* **[!UICONTROL IP-Adressen blockieren]**: Verhindert, dass bestimmte IPs auf Marketo zugreifen.
   >* **[!UICONTROL IP-Einschränkungen deaktivieren]**: Wenn Sie dies überprüfen, funktionieren alle/alle Einschränkungsregeln nicht mehr. Verwenden Sie dies zu Testzwecken.

   >[!NOTE]
   >
   >Sie können mehrere Einschränkungen hinzufügen, diese können jedoch nur &quot;ALLE&quot;oder &quot;ALLE blockiert&quot;sein. Sie können nicht mischen und passend erlaubt und blockiert.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Ihre Marketing-Daten sind jetzt sicherer als je zuvor!
