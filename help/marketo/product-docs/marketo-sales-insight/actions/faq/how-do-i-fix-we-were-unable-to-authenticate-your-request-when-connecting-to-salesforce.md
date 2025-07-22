---
description: Wie kann ich das Problem beheben, dass wir Ihre Anfrage nicht authentifizieren konnten, als wir eine Verbindung zu Salesforce herstellen - Marketo-Dokumente - Produktdokumentation
title: Wie kann ich das Problem beheben, dass wir Ihre Anfrage beim Herstellen einer Verbindung mit Salesforce nicht authentifizieren konnten?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Wie kann ich das Problem beheben, dass wir Ihre Anfrage beim Herstellen einer Verbindung mit [!DNL Salesforce] nicht authentifizieren konnten? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie versuchen, Ihre Marketo-Verkaufsinstanz mit Salesforce zu verbinden und der Fehler „Wir können Ihre Anfrage nicht authentifizieren“ angezeigt wird, hängt dies wahrscheinlich mit der Konfiguration Ihrer Salesforce-Instanz zusammen.

Es gibt zwei Arten von Fehlern, die diese fehlgeschlagene Authentifizierungsseite erzeugen können.

* Anmeldefehler - Eingeschränkte Domain
* OAuth-App blockiert

Sie können feststellen, welchen Typ Sie erhalten, indem Sie die URL überprüfen.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Beheben des Anmeldefehlers Eingeschränkte Domain {#resolve-login-error-restricted-domain}

Dieser Fehler weist in der Regel darauf hin, dass Sie über eine benutzerdefinierte Domain verfügen, zu der wir keine Route durchführen können. Um diesen Fehler zu beheben, versuchen Sie, sich bei der Salesforce-Instanz anzumelden, mit der Sie eine Verbindung herstellen möchten. Führen Sie dann die Schritte aus, um eine Verbindung zu Salesforce herzustellen.

Wenn die Instanz, zu der Sie eine Verbindung herstellen möchten, eine Salesforce Sandbox-Domain ist und Sie einen Fehler erhalten, müssen Sie zusätzliche Schritte ausführen, um Ihre Instanz so zu aktualisieren, dass sie mit Salesforce Sandbox kompatibel ist. [Weitere Informationen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Beheben einer blockierten OAuth-App {#resolve-oauth-app-blocked}

Wenn Sie die Fehlermeldung „Wir konnten Ihre Anfrage nicht authentifizieren“ mit dem Fehlertyp „OAuth App Blocked“ (oder einem anderen Typ) in der URL erhalten haben, kann dies zu einer Einschränkung Ihres Zugriffs auf die API von Salesforce führen. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass die folgenden Voraussetzungen erfüllt sind.

### Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen Salesforce-Administrator, sich bei Salesforce anzumelden.
1. Wählen Sie **Setup** aus.
1. Wählen Sie **Benutzer verwalten** aus.
1. Wählen Sie **Profile** aus.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Scrollen Sie nach unten **Administratorberechtigungen** und stellen Sie sicher, dass **API aktiviert** aktiviert ist.

### Überprüfen Sie, ob Salesforce Sales Insight-Aktionen am Herstellen einer Verbindung hindert {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Bitten Sie einen Salesforce-Administrator, sich bei Salesforce anzumelden.
1. Wählen Sie **Setup** aus.
1. Wählen Sie **Apps verwalten** aus.
1. Wählen Sie **Connected Apps OAuth Usage** aus.
1. Stellen Sie sicher, dass neben Sales Insight Actions „Block“ angezeigt wird. Wenn Sie „Blockierung aufheben“ sehen, klicken Sie auf die Schaltfläche, um den Zugriff von Sales Insight Actions auf Salesforce aufzuheben.
