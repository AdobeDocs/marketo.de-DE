---
unique-page-id: 2360185
description: Kennwortsicherheitseinstellungen ändern - Marketo-Dokumente - Produktdokumentation
title: Kennwortsicherheitseinstellungen ändern
exl-id: cda7ec70-32aa-4e0a-86b2-eb9bea70ef72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Kennwortsicherheitseinstellungen ändern {#change-your-password-security-settings}

Steuern Sie die Kennwortrichtlinie Ihres Abonnements. So geht es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. under **Admin** klicken **Anmeldeeinstellungen**.

   ![](assets/image2014-9-16-12-3a41-3a40.png)

1. under **Sicherheitseinstellungen** klicken **Bearbeiten**.

   ![](assets/passwordsettings-hand.png)

1. Wählen Sie eine **Vorlage**. Für erweiterte Optionen klicken Sie auf **Erweitert** Dropdown-Liste.

   >[!NOTE]
   >
   >Eine Vorlage ist nur eine vordefinierte Konfiguration. Standard ist gut. Hohe Sicherheit ist die stärkste. Mit Benutzerdefiniert können Sie Ihre eigenen erstellen.

   ![](assets/passwordstrength.png)

   >[!TIP]
   >
   >In **Benutzerdefiniert** aktivieren, aktivieren Sie die Kontrollkästchen, um anzugeben, welche Merkmale Benutzer bei der Erstellung von Passwörtern einbeziehen sollen.

1. Legen Sie die **Ablauf**. Für diese Funktion müssen Benutzer ihre Kennwörter nach einer bestimmten Zeitdauer automatisch zurücksetzen. Dies schließt auch den Admin-Benutzer ein.

   >[!CAUTION]
   >
   >Vorhandene Benutzer werden nicht über die Änderungen informiert. Satz **Ablauf** auf 30 Tage zu setzen, um sicherzustellen, dass alle auf die neuen Einstellungen aktualisiert haben, und diese dann wieder in Ihre ursprüngliche Kadenz ändern.

   ![](assets/expiration.png)

1. Legen Sie die **Inaktives Sitzungs-Timeout**. Dadurch wird bestimmt, wie lange ein Benutzer inaktiv sein kann, bevor er sich erneut bei Marketo anmelden muss.

   ![](assets/inactivesession.png)

   Sicherheit ist ein ernstes Geschäft. Wir haben dir den Rücken geschlagen.
