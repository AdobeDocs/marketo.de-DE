---
description: Wie behebe ich die Fehlermeldung "Wir konnten Ihre Anfrage nicht authentifizieren"bei der Verbindung mit Salesforce - Marketo Docs - Produktdokumentation
title: Wie behebe ich bei der Verbindung mit Salesforce die Fehlermeldung "Wir konnten Ihre Anfrage nicht authentifizieren"?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: b09bff5fe72e5cce86ab4664e264edb181fa3e5c
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Wie behebe ich bei der Verbindung mit Salesforce die Fehlermeldung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie versuchen, Ihre Marketo Sales-Instanz mit Salesforce zu verbinden, und der Fehler &quot;Wir können Ihre Anfrage nicht authentifizieren&quot;angezeigt wird, hängt dies wahrscheinlich mit der Konfiguration Ihrer Salesforce-Instanz zusammen.

Es gibt zwei Arten von Fehlern, die diese fehlgeschlagene Authentifizierungsseite verursachen können.

* Anmeldefehler - Domain eingeschränkt
* OAuth App blockiert

Sie können ermitteln, welchen Typ Sie erhalten, indem Sie die URL überprüfen.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Beheben von Anmeldefehlern - Eingeschränkte Domäne {#resolve-login-error-restricted-domain}

Dieser Fehler zeigt normalerweise an, dass Sie über eine benutzerdefinierte Domäne verfügen, zu der wir keine Weiterleitung durchführen können. Um diesen Fehler zu beheben, versuchen Sie, sich bei der Salesforce-Instanz anzumelden, mit der Sie zuerst eine Verbindung herstellen möchten. Gehen Sie dann die Schritte durch, um eine Verbindung mit Salesforce herzustellen.

Wenn es sich bei der Instanz, mit der Sie eine Verbindung herstellen möchten, um eine Salesforce-Sandbox-Domäne handelt und Sie einen Fehler erhalten, müssen Sie zusätzliche Schritte ausführen, um Ihre Instanz so zu aktualisieren, dass sie mit Salesforce Sandbox kompatibel ist. [Weitere Informationen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Beheben von blockierten OAuth-Apps und anderen Fehlertypen {#resolve-oauth-app-blocked-and-other-error-types}

Wenn Sie die Fehlermeldung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;mit dem Fehlertyp Oauth App Blocked oder einem anderen Typ in der URL erhalten, besteht möglicherweise eine Einschränkung Ihres Zugriffs auf die Salesforce-API. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass die folgenden Elemente vorhanden sind.

### Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen Salesforce-Administrator, sich bei Salesforce anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Benutzer verwalten**.
1. Auswählen **Profile**.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Nach unten scrollen zu **Administratorberechtigungen** und stellen Sie sicher, **API aktiviert** aktiviert ist.

### Überprüfen Sie, ob Salesforce Sales Insight-Aktionen von der Verbindung blockiert {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Bitten Sie einen Salesforce-Administrator, sich bei Salesforce anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Apps verwalten**.
1. Auswählen **Connected Apps OAuth-Nutzung**.
1. Stellen Sie sicher, dass Sales Insight-Aktionen daneben &quot;Block&quot;anzeigen. Wenn &quot;Block aufheben&quot;angezeigt wird, klicken Sie auf die Schaltfläche , um den Zugriff von Sales Insight-Aktionen auf Salesforce zu entsperren.
