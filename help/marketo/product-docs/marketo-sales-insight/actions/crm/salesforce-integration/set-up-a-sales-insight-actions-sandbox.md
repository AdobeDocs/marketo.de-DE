---
description: Einrichten einer Insight-Aktions-Sandbox für den Vertrieb - Marketo-Dokumente - Produktdokumentation
title: Einrichten einer Sandbox für Sales Insight Actions
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 2%

---

# Einrichten einer Sandbox für Sales Insight Actions {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions ist ein Web-basiertes Programm, das über das [Marketo Sales Insight Package&rbrace; ausschließlich mit dem Salesforce CRM integriert ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Dies wird manchmal als &quot;Marketo-Vertrieb“ oder einfach als „Aktionen“ bezeichnet.

Wenn Sie über eine Marketo-Sandbox verfügen, können Sie die Verwendung einer Actions-Instanz mit Ihrer Sandbox zu Testzwecken aktivieren.

Beim Einrichten einer Aktionsinstanz müssen Sie entscheiden, ob sie für die Verwendung mit Salesforce Sandbox oder Salesforce Production konfiguriert werden soll. Dies liegt daran, dass Salesforce jeweils unterschiedliche Endpunkte verwendet und Actions die Verbindung zu Salesforce zum Aktivieren und Authentifizieren von Benutzenden nutzt.

Gehen Sie wie folgt vor, um eine Actions-Instanz für die Zusammenarbeit mit Ihrer Salesforce Sandbox-Instanz einzurichten.

>[!NOTE]
>
>Erfahren Sie mehr darüber, wie Benutzer ihren [ aktivieren ](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. Außerdem erfahren Sie, wie sich Benutzer [bei Salesforce authentifizieren](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Wenn Sie es vorziehen, Benutzer per E-Mail und Kennwort authentifizieren zu lassen, können Sie mehr darüber in unserem Artikel [Login Management Settings](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"} erfahren.

## Anfordern einer Aktionsinstanz zur Bereitstellung in Ihrer Marketo-Sandbox {#request=an-actions-instance}

Sales Insight Actions ist nur auf Anfrage für Marketo Sandbox-Instanzen aktiviert. Wenden Sie sich an das Adobe Account Team (Ihren Account Manager), um eine Anfrage zu senden.

## Bereitstellen Ihres Aktionskontos für Marketo Sandbox {#provision-your-actions-account}

Sobald Aktionen für Ihre Marketo-Sandbox aktiviert ist, müssen Sie die folgenden Schritte ausführen, um Ihre neue Instanz zu aktivieren.

1. Melden Sie sich bei Ihrer Marketo Sandbox-Instanz an.

1. Navigieren Sie zu **Admin**.

1. Wählen Sie **Sales Insight** aus.

1. Wählen Sie **Aktionskonfiguration** aus.

   >[!IMPORTANT]
   >
   >Eine E-Mail-Adresse kann über Sandbox- und Produktionsinstanzen hinweg nur für eine Aktionsinstanz verwendet werden. Wenn Sie ein Administrator sind, der Zugriff auf mehrere Instanzen in Produktion und Sandbox benötigt, müssen Sie für jede Instanz eine andere E-Mail-Adresse verwenden.

1. Wählen Sie auf der Bereitstellungskarte den Benutzer aus, den Sie in Ihre Sales Insight Actions-Instanz einladen möchten.

## Aktivieren der Aktionsinstanz {#activate-your-actions-instance}

Ihre Actions-Instanz muss mit einem Salesforce-Produktionskonto aktiviert werden. Nachdem er aktiviert wurde, kann er zu einem Salesforce Sandbox-Konto gewechselt werden.

1. Suchen Sie die gesendete Einladung.

1. Klicken Sie auf **Link „Erste**&quot;.

1. Aktivieren Sie mit Ihrer Salesforce-Produktionsinstanz.

1. Befolgen Sie die Anweisungen, um das Konto einzurichten. Einen detaillierten Überblick erhalten Sie in unserem Artikel [User Onboarding](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Vorbereiten der Aktionsinstanz auf die Kompatibilität mit der Salesforce Sandbox-Instanz {#prepare-your-actions-instance}

Für „Aktionen“ müssen Sie zunächst eine neue Instanz bei einem Salesforce-Produktionsbenutzer aktivieren. Nach der Aktivierung können Sie die folgenden Schritte ausführen, um Ihre Instanz so vorzubereiten, dass sie mit Salesforce Sandbox kompatibel ist.

1. Aktualisieren Sie die Anmeldeeinstellungen auf „Alle Anmeldemethoden“, damit Sie sich bei Bedarf mit einem Benutzernamen und Kennwort anmelden können. Wenn gewünscht, kann dies wieder auf „Nur Salesforce&quot; umgeschaltet werden, nachdem alles konfiguriert wurde. [Weitere Informationen dazu finden Sie hier](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Trennen Sie die Verbindung zur Salesforce-Produktion und stellen Sie eine Verbindung zur Salesforce-Sandbox her. [Hier erfahren Sie, wie Sie eine Verbindung herstellen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. Wählen Sie für Schritt 3 „Sandbox“ anstelle von &quot;Salesforce&quot; aus. Wenn Sie bereits verbunden sind, sollte auf der Registerkarte Salesforce-Verbindungen und -Anpassungen eine Option zum Trennen angezeigt werden.

>[!NOTE]
>
>Wenn Sie über eine benutzerdefinierte Domain für Ihre Salesforce-Instanz verfügen, empfehlen wir, sich bei Ihrer Salesforce-Instanz anzumelden, bevor Sie eine Verbindung zu Salesforce herstellen oder sich bei Actions anmelden.

## Anfordern der Konvertierung Ihrer Aktionsinstanz, damit sie mit Ihrer Salesforce-Sandbox kompatibel ist {#request-your-actions-instance-be-converted}

1. Wenden Sie sich an den [Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}Support, um Ihre neue Sales Insight Actions-Instanz so zu konfigurieren, dass sie mit Salesforce Sandbox kompatibel ist.

1. Testen Sie, ob alles richtig konfiguriert ist, indem Sie versuchen, sich mit der Schaltfläche „Mit Salesforce anmelden“ auf der Seite toutapp.com/login anzumelden.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Wenn an dieser Stelle Probleme auftreten, können Sie das Zurücksetzen des Kennworts anfordern und mithilfe eines Kennworts den Zugriff auf Ihr Konto wiederherstellen.

Jetzt kann Ihre Instanz mit Ihrer Salesforce Sandbox-Instanz verwendet werden. Wenn Sie die automatische Anmeldung von [Salesforce ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}Salesforce verwenden möchten, können Sie in Ihren [Anmeldeverwaltungseinstellungen“ auf „Nur Salesforce&quot; ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Verbinden Ihres Sales Insight Actions-Kontos mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Benutzerhandbuch zum Onboarding von Sales Insight-Aktionen](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Automatische Anmeldung über Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Einstellungen für die Anmeldeverwaltung](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
