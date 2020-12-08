---
unique-page-id: 2952678
description: Verwenden Sie das Token "Warnhinweisinformationen senden"{SP_Send_Alert_Info} - "Marketing to Docs"- Produktdokumentation
title: Verwenden des Tokens "Warnhinweisinformationen senden"
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Verwenden des Tokens &quot;Warnhinweisinformationen senden&quot; {#use-the-send-alert-info-token-sp-send-alert-info}

Das `{{SP_Send_Alert_Info}}` Token ist ein spezielles Token, das beim Erstellen von Warn-E-Mails für Ihr Vertriebsteam verwendet wird.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!TIP]
>
>Dieses Token funktioniert nur wie gewünscht, wenn die E-Mail mit dem Textfluss &quot;Warnung [senden](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) &quot;gesendet wird. Es funktioniert nicht, wenn es in einem Schritt zum Senden einer E-Mail-Benachrichtigung verwendet wird.

Beispiel-Warnung:   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Kopf hoch! URLs in Warnungen haben Ablaufdaten, um sicherzustellen, dass sie über eine Kadenz verfügen, die diese Arten von Nachrichten unterstützt. Ablaufdaten werden von einem Administrator [konfiguriert](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Die folgenden Informationen sind Teil der `{{SP_Send_Alert_Info}}`:

* Vorname und Nachname als Link zu den Personendetails in Marketo
* Ein Link zur Person in Ihrem CRM-System
* Der Name der Kampagne in Marketo, die die Warnung gesendet hat
* Zeitpunkt der Versendung der Ausschreibung

>[!NOTE]
>
>Der Link zum CRM erscheint nur, wenn sich die Person im CRM-System befindet (derzeit nicht mit Dynamics CRM verfügbar). Der Link ist sowohl für Marketo- als auch für Nicht-Marketo-Benutzer zugänglich.

## hinzufügen des Tokens SP_Send_Alert_Info an eine E-Mail {#add-the-sp-send-alert-info-token-to-an-email}

1. Wählen Sie die E-Mail aus und klicken Sie auf Entwurf **bearbeiten**.

   ![](assets/one-3.png)

1. Klicken Sie bei gedrückter Dublette auf den bearbeitbaren Bereich, dem Sie das Token hinzufügen möchten.

   ![](assets/two-3.png)

1. Platzieren Sie den Cursor an der Stelle, an der das Token stehen soll, und klicken Sie dann auf die Schaltfläche &quot;Token **einfügen&quot;** .

   ![](assets/three-3.png)

1. Suchen und wählen Sie das **`{{SP_Send_Alert_Info}}`** Token aus und klicken Sie auf **Einfügen**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Erinnerung**
>
>Vergiss nicht, deine E-Mail zu genehmigen!

Gut! Dieses Token ist sehr nützlich und Sie sollten es in allen Warnungen verwenden, die Sie für Ihr Verkaufsteam erstellen.