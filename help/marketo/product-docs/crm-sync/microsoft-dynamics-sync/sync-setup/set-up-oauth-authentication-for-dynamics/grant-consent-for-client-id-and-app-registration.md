---
description: Genehmigung für Client-ID und App-Registrierung - Marketo Docs - Produktdokumentation
title: Genehmigung für Client-ID und App-Registrierung
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Genehmigung für Client-ID und App-Registrierung {#grant-consent-for-client-id-and-app-registration}

## Delegierte Benutzerberechtigungen für den Synchronisierungsbenutzer {#grant-delegated-user-permissions-for-the-sync-user} gewähren

1. Verwenden Sie ein sauberes Programm (Notepad für Windows, Textbearbeitung für Mac), um einen URI (Uniform Resource Identifier) für die Autorisierung zu erstellen, indem Sie den Untertext einfügen und die Werte client_id, redirect_uri und stae ersetzen.

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
      <td>sollte client_id sein, das im App-Registrierungsprozess generiert wurde</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri-Wert</strong></td> 
      <td>sollte mit dem Wert identisch sein, der zum Zeitpunkt der App-Registrierung &gt; Weiterleitungs-URIs eingegeben wurde</td> 
     </tr> 
     <tr> 
      <td><strong>Statuswert</strong></td> 
      <td>kann eine beliebige ID sein (z. B. 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   Die endgültige URL sollte etwa wie folgt aussehen: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Öffnen Sie den von Ihnen erstellten URI in einem beliebigen Browser.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Melden Sie sich als Synchronisierungsbenutzer an, für den Sie Berechtigungen erteilen.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Wenn Sie bereits in einem anderen Register als Administrator angemeldet sind, müssen Sie einen anderen Browser oder Inkognito-Modus verwenden, um sich als Synchronisierungsbenutzer anzumelden.

1. Klicken Sie auf **Accept**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Zustimmung für alle Benutzer {#grant-consent-for-all-users}

Als Administrator können Sie auch die delegierten Berechtigungen einer Anwendung für alle Benutzer in Ihrem Mandanten genehmigen. Die behördliche Zustimmung verhindert, dass der Dialog über die Zustimmung für jeden Benutzer im Mieter erscheint, und kann im Azurblauen Portal von Benutzern mit der Administratorrolle durchgeführt werden. Erfahren Sie, welche Administratorrollen [die Zustimmung zu delegierten Berechtigungen hier](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference) erteilen können.

1. Navigieren Sie in Ihrem Azurblauen Portal zur Anwendungshomepage.

1. Klicken Sie unter Verwalten auf **API-Berechtigungen**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Klicken Sie auf die Schaltfläche **Administratorgenehmigung gewähren** (für Mandanten).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Klicken Sie zur Bestätigung auf **Ja**.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[Einrichten der Microsoft Dynamics CRM-App für On-Prem](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
