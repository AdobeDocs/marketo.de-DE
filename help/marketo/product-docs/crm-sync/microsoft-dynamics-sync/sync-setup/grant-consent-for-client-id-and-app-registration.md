---
description: Einverständnis für Client-ID und App-Registrierung erteilen - Marketo-Dokumente - Produktdokumentation
title: Erteilen von Einverständnis für Client-ID und App-Registrierung
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 6%

---

# Erteilen von Einverständnis für Client-ID und App-Registrierung {#grant-consent-for-client-id-and-app-registration}

Gehen Sie wie folgt vor, um zu erfahren, wie Sie die erforderlichen Einverständnisse/Berechtigungen erteilen.

## Gewähren von delegierten Benutzerberechtigungen für den Synchronisierungsbenutzer {#grant-delegated-user-permissions-for-the-sync-user}

1. Verwenden Sie ein Textverarbeitungsprogramm (Editor für Windows, Textbearbeitung für Mac), um einen URI (Uniform Resource Identifier) für die Autorisierung zu erstellen, indem Sie den folgenden Text einfügen und die Werte `client_id`, `redirect_uri` und `state` ersetzen.

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
      <td><strong>client_id value</strong></td>
      <td>sollte die im Prozess zur App-Registrierung generierte client_id sein</td>
     </tr>
     <tr>
      <td><strong>Wert für redirect_uri</strong></td>
      <td>sollte mit dem Wert übereinstimmen, der zum Zeitpunkt der App-Registrierung &gt; Umleitungs-URIs eingegeben wurde</td>
     </tr>
     <tr>
      <td><strong>Zustandswert</strong></td>
      <td>kann eine beliebige ID sein (z. B. 12345)</td>
     </tr>
    </tbody>
   </table>

   Die endgültige URL sollte in etwa wie folgt aussehen: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Öffnen Sie den erstellten URI in einem beliebigen Browser.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Melden Sie sich als Synchronisierungsbenutzer an, für den Sie Berechtigungen erteilen.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Wenn Sie bereits auf einer anderen Registerkarte als Administrator bei Azure angemeldet sind, müssen Sie einen anderen Browser oder Inkognito-Modus verwenden, um sich als Synchronisierungsbenutzer anzumelden.

1. Klicken Sie **[!UICONTROL Akzeptieren]**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Einverständnis für alle Benutzer erteilen {#grant-consent-for-all-users}

Als Admin können Sie auch den delegierten Berechtigungen einer Anwendung im Namen aller Benutzenden in Ihrem Mandanten zustimmen. Die administrative Zustimmung verhindert, dass das Einverständnisdialogfeld für jeden Benutzer im Mandanten angezeigt wird, und kann im Azure-Portal von Benutzern mit Administratorrolle vorgenommen werden. Hier erfahren Sie, welche Administratorrollen [hier delegierten Berechtigungen zustimmen](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Navigieren Sie in Ihrem Azure-Portal zur Startseite der Anwendung.

1. Klicken [!UICONTROL  unter &quot;]&quot; auf **[!UICONTROL API-]**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Klicken Sie auf **[!UICONTROL Schaltfläche „Administratorzustimmung erteilen]** (für Mandanten).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Klicken Sie **[!UICONTROL Ja]** zur Bestätigung.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)
