---
unique-page-id: 8783322
description: Validieren von Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync überprüfen
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Überprüfen der Microsoft Dynamics-Synchronisierung {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Wenn Multi-Factor Authentication (MFA) für die Dynamiksynchronisierung aktiviert ist, müssen Sie diese deaktivieren, damit Dynamics mit Marketo ordnungsgemäß synchronisiert werden kann. Weitere Informationen erhalten Sie beim [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

## Synchronisierung in Marketo überprüfen{#run-validate-sync-in-marketo}

Es ist sehr wichtig, dass Sie das Tool zum Überprüfen der Synchronisierung ausführen, um sicherzustellen, dass Microsoft Dynamics Sync mit Marketo korrekt eingerichtet ist, bevor Sie die letzte Verbindung herstellen. Der Prozess generiert eine Checkliste mit sieben Setup-Schritten, die bestimmen, wo Probleme auftreten. Die Überprüfung, ob diese ordnungsgemäß durchgeführt wurden, kann viel Zeit später einsparen.

1. Klicken Sie auf die Registerkarte **Admin** und dann auf den Link **Microsoft Dynamics** im Bereich Integration.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Wählen Sie **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicken Sie auf die Registerkarte **Synchronisierungseinstellungen überprüfen**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Geben Sie Ihren Benutzernamen, Ihr Kennwort und Ihre URL ein (Client-ID und geheimer Clientschlüssel sind optional). Klicken Sie abschließend auf **Weiter**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Wenn Sie zuvor synchronisiert haben, wird **CRM** in der linken Struktur **Microsoft Dynamics** gelesen und die Daten im obigen Formular können vorausgefüllt werden.

1. Wenn alles in Ordnung ist, generiert die Synchronisierung validieren eine Checkliste mit grünen Markierungen ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Wenn ein ![—](assets/delete.png) angezeigt wird, liegt ein Problem bei diesem Schritt vor. Weitere Informationen zum Identifizieren und Beheben des Problems finden Sie unter [Probleme bei der Synchronisierung der Dynamikvalidierung ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) beheben. Führen Sie dann die Synchronisierungsüberprüfungsschritte erneut aus, bis das Ergebnis wie das Bild oben aussieht.

   >[!CAUTION]
   >
   >Die Sandbox-Aktualisierung für Marketo Dynamics Sync wird derzeit nicht unterstützt. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, benötigen Sie eine neue Marketo-Sandbox. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.

>[!MORELIKETHIS]
>
>[Probleme mit der Synchronisierung der Dynamikvalidierung beheben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
