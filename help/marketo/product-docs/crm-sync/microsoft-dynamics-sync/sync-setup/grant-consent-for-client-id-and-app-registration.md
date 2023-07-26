---
description: Erteilen der Zustimmung für die Client-ID und App-Registrierung - Marketo Docs - Produktdokumentation
title: Erteilen der Zustimmung für die Kunden-ID und App-Registrierung
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Erteilen der Zustimmung für die Kunden-ID und App-Registrierung {#grant-consent-for-client-id-and-app-registration}

## Delegierte Benutzerberechtigungen für den Synchronisierungsbenutzer gewähren {#grant-delegated-user-permissions-for-the-sync-user}

1. Verwenden Sie ein sauberes Textprogramm (Notepad für Windows, Textbearbeitung für Mac), um eine URI (Uniform Resource Identifier) für die Autorisierung zu erstellen, indem Sie den unten stehenden Text einfügen und die Werte client_id, redirect_uri und geben.

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>client_id-Wert</strong></td> 
      <td>sollte die im App-Registrierungsprozess generierte client_id sein.</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri-Wert</strong></td> 
      <td>sollte mit dem Wert übereinstimmen, der zum Zeitpunkt der App-Registrierung &gt; Weiterleitungs-URIs eingegeben wurde</td> 
     </tr> 
     <tr> 
      <td><strong>Statuswert</strong></td> 
      <td>kann eine beliebige ID sein (z. B. 12345).</td> 
     </tr> 
    </tbody> 
   </table>

   Die endgültige URL sollte ungefähr so aussehen: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Öffnen Sie den von Ihnen erstellten URI in einem beliebigen Browser.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Melden Sie sich als Synchronisierungsbenutzer an, für den Sie Berechtigungen erteilen.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Wenn Sie bereits auf einer anderen Registerkarte bei Azure als Administrator angemeldet sind, müssen Sie einen anderen Browser oder Inkognito-Modus verwenden, um sich als Synchronisierungsbenutzer anzumelden.

1. Klicks **Accept**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Zustimmung für alle Benutzer erteilen {#grant-consent-for-all-users}

Als Administrator können Sie auch die delegierten Berechtigungen einer Anwendung im Namen aller Benutzer in Ihrem Mandanten genehmigen. Die administrative Zustimmung verhindert, dass das Dialogfeld für die Zustimmung für jeden Benutzer im Mandanten angezeigt wird, und kann im Azure-Portal von Benutzern mit der Administratorrolle ausgeführt werden. Erfahren Sie, welche Administratorrollen verfügbar sind [Zustimmung zu delegierten Berechtigungen hier](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Navigieren Sie in Ihrem Azure-Portal zur Startseite der Anwendung.

1. Klicken Sie unter Verwalten auf **API-Berechtigungen**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Klicken Sie auf **Erteilen der Admin-Zustimmung** (für Mandanten).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Klicks **Ja** zur Bestätigung.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

