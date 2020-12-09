---
unique-page-id: 8783322
description: Validieren von Microsoft Dynamics Sync - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync überprüfen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Microsoft Dynamics Sync überprüfen {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Wenn Multi-Factor Authentication (MFA) für die Dynamiksynchronisierung aktiviert ist, müssen Sie sie deaktivieren, damit Dynamics mit Marketo richtig synchronisiert wird. Für weitere Informationen wenden Sie sich bitte an [den Marketing](http://nation.marketo.com/community/support_solutions)Support.

## Synchronisierung in Marketing überprüfen {#run-validate-sync-in-marketo}

Es ist sehr wichtig, dass Sie das Tool zum Überprüfen der Synchronisierung ausführen, um sicherzustellen, dass Microsoft Dynamics Sync mit Marketo korrekt eingerichtet ist, bevor Sie die letzte Verbindung herstellen. Der Prozess generiert eine Checkliste mit sieben Setup-Schritten, die bestimmen, wo Probleme auftreten. Die Überprüfung, ob diese ordnungsgemäß durchgeführt wurden, kann viel Zeit später einsparen.

1. Klicken Sie auf die Registerkarte **Admin** und dann auf den Link **Microsoft Dynamics** im Bereich Integration.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Wählen Sie **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicken Sie auf die Registerkarte **Synchronisierungseinstellungen überprüfen** .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Geben Sie Ihren Benutzernamen, Ihr Kennwort und Ihre URL ein (Client-ID und geheimer Clientschlüssel sind optional). Klicken Sie abschließend auf **Weiter** .

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Wenn Sie zuvor synchronisiert haben, liest **CRM** im linken Baum **Microsoft Dynamics**, und die Daten im obigen Formular können vorausgefüllt werden.

1. Wenn alles in Ordnung ist, generiert die Synchronisierung überprüfen eine Checkliste mit grünen Auswahlfeldern ![-](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Wenn ein ![—](assets/delete.png)angezeigt wird, liegt ein Problem bei diesem Schritt vor. Informationen zum Identifizieren und Beheben des Problems finden Sie unter Probleme mit der Synchronisierung bei der [Synchronisierung der Dynamikvalidierung](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) beheben. Führen Sie dann die Synchronisierungsüberprüfungsschritte erneut aus, bis das Ergebnis wie das Bild oben aussieht.

   >[!CAUTION]
   >
   >Wir unterstützen derzeit keine Sandbox-Aktualisierung für Marketo Dynamics Sync. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, benötigen Sie eine neue Marketo-Sandbox. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.

>[!MORELIKETHIS]
>
>[Probleme mit der Synchronisierung der Dynamikvalidierung beheben](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

