---
description: Einrichten einer Sandbox für Einblicke in Verkaufsaktionen - Marketo-Dokumente - Produktdokumentation
title: Einrichten einer Sandbox für Einblicke in Verkaufsaktionen
exl-id: 58af77ef-93ea-4149-be91-f86cdc8f7476
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Einrichten einer Sandbox für Einblicke in Verkaufsaktionen {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions ist eine webbasierte Anwendung, die über die [Marketo Sales Insight-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Dies wird manchmal als &quot;Marketo-Verkäufe&quot;oder einfach als &quot;Aktionen&quot;bezeichnet.

Wenn Sie über eine Marketo-Sandbox verfügen, können Sie zu Testzwecken eine Aktionsinstanz für Ihre Sandbox aktivieren.

Beim Einrichten einer Aktionsinstanz müssen Sie entscheiden, ob sie für die Verwendung mit Salesforce Sandbox oder Salesforce-Produktion konfiguriert wird. Dies liegt daran, dass Salesforce für jeden einzelnen Endpunkt verschiedene Endpunkte verwendet und Aktionen die Verbindung zu Salesforce zum Aktivieren und Authentifizieren von Benutzern verwendet.

Gehen Sie wie folgt vor, um eine Aktionsinstanz für die Arbeit mit Ihrer Salesforce Sandbox-Instanz einzurichten.

>[!NOTE]
>
>Weitere Informationen dazu, wie Benutzer [Setzen der Aktionen aktivieren](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. You can also learn about how users will [authenticate with Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Additionally, if you prefer to have users authenticate with email and password, you can learn more about this in our [Login Management settings article](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Anfordern einer Aktionsinstanz zur Bereitstellung für Ihre Marketo-Sandbox {#request=an-actions-instance}

Sales Insight-Aktionen sind für Marketo-Sandbox-Instanzen nur auf Anfrage aktiviert. Wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), um eine Anfrage zu senden.

## Bereitstellen Ihres Aktionskontos für Marketo Sandbox {#provision-your-actions-account}

Sobald Aktionen für Ihre Marketo-Sandbox aktiviert sind, müssen Sie die folgenden Schritte ausführen, um Ihre neue Instanz zu aktivieren.

1. Melden Sie sich bei Ihrer Marketo-Sandbox-Instanz an.

1. Navigieren Sie zu **Admin**.

1. Auswählen **Sales Insight**.

1. Auswählen **Aktionskonfiguration**.

   >[!IMPORTANT]
   >
   >Eine E-Mail-Adresse kann nur für eine Aktionsinstanz über Sandbox- und Produktionsinstanzen hinweg verwendet werden. Wenn Sie ein Administrator sind, der Zugriff auf mehrere Instanzen in der gesamten Produktion und Sandbox benötigt, müssen Sie für jede Instanz eine andere E-Mail-Adresse verwenden.

1. Wählen Sie auf der Bereitstellungskarte den Benutzer aus, den Sie zu Ihrer Sales Insight-Aktionsinstanz einladen möchten.

## Aktivieren Ihrer Aktionsinstanz {#activate-your-actions-instance}

Ihre Aktionsinstanz muss mit einem Salesforce-Produktionskonto aktiviert werden. Nach der Aktivierung kann es zu einem Salesforce-Sandbox-Konto gewechselt werden.

1. Suchen Sie die gesendete Einladung.

1. Klicken Sie auf **Erste Schritte** Link.

1. Aktivieren Sie mit Ihrer Salesforce-Produktionsinstanz.

1. Befolgen Sie die Anweisungen zum Einrichten des Kontos. Eine ausführliche Übersicht finden Sie in unserer [Artikel zur Benutzerintegration](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Vorbereiten Ihrer Aktionsinstanz auf Kompatibilität mit Ihrer Salesforce-Sandbox-Instanz {#prepare-your-actions-instance}

Für Aktionen müssen Sie zuerst eine neue Instanz mit einem Salesforce-Produktionsbenutzer aktivieren. Nach der Aktivierung können Sie die folgenden Schritte ausführen, um Ihre Instanz auf die Kompatibilität mit Salesforce Sandbox vorzubereiten.

1. Aktualisieren Sie die Anmeldeeinstellungen auf &quot;Alle Anmeldemethoden&quot;, damit Sie sich bei Bedarf mit einem Benutzernamen und einem Kennwort anmelden können. Wenn dies gewünscht wird, kann nach der Konfiguration aller Elemente wieder auf &quot;Nur Salesforce&quot;umgestellt werden. [Hier erfahren Sie, wie Sie das machen.](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Trennen Sie die Verbindung zur Salesforce-Produktion und stellen Sie eine Verbindung zu Ihrer Salesforce-Sandbox her. [Hier erfahren Sie, wie Sie eine Verbindung herstellen](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. Wählen Sie für Schritt 3 &quot;Sandbox&quot;anstelle von &quot;Salesforce&quot;aus. Wenn Sie bereits eine Verbindung hergestellt haben, sollten Sie auf der Registerkarte Salesforce-Verbindungen und -Anpassungen eine Option zum Trennen der Verbindung sehen.

>[!NOTE]
>
>Wenn Sie über eine benutzerdefinierte Domäne für Ihre Salesforce-Instanz verfügen, empfehlen wir, sich bei Ihrer Salesforce-Instanz anzumelden, bevor Sie eine Verbindung zu Salesforce herstellen oder sich bei Aktionen anmelden.

## Anfordern der Konvertierung Ihrer Aktionsinstanz in die Kompatibilität mit Ihrer Salesforce-Sandbox {#request-your-actions-instance-be-converted}

1. Kontakt [Marketo Engage-Unterstützung](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} , um Ihre neue Instanz von Sales Insight Actions anzufordern, damit sie mit der Salesforce-Sandbox kompatibel ist.

1. Testen Sie alles ordnungsgemäß, indem Sie versuchen, sich über die Schaltfläche &quot;Mit Salesforce anmelden&quot;auf der Seite toutapp.com/login anzumelden.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Wenn zu diesem Zeitpunkt Probleme auftreten, können Sie eine Zurücksetzung des Kennworts anfordern und ein Kennwort verwenden, um den Zugriff auf Ihr Konto wiederherzustellen.

Jetzt kann Ihre Instanz mit Ihrer Salesforce-Sandbox-Instanz verwendet werden. Wenn Sie [Automatische Salesforce-Anmeldung](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} from Salesforce, you can switch back to "Salesforce Only" in your [Login Management settings](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Verbinden Ihres Sales Insight-Aktionskontos mit Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Benutzerhandbuch zu Insight-Maßnahmen für Vertrieb](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Automatische Anmeldung über Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Anmeldeverwaltungseinstellungen](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
