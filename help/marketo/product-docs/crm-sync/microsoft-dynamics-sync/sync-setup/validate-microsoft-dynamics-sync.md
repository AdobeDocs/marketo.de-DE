---
unique-page-id: 8783322
description: Validieren [!DNL Microsoft Dynamics] Synchronisieren - Marketo-Dokumente - Produktdokumentation
title: validate [!DNL Microsoft Dynamics] sync
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Validieren [!DNL Microsoft Dynamics] Synchronisieren {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Wenn Sie die Multi-Factor Authentication (MFA) für Ihre [!DNL Dynamics]-Synchronisierung aktiviert haben, müssen Sie sie deaktivieren, damit [!DNL Dynamics] ordnungsgemäß mit Marketo synchronisieren können. Weitere Informationen erhalten Sie vom [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

## Ausführen von „Synchronisierung validieren“ in Marketo {#run-validate-sync-in-marketo}

Es ist sehr wichtig, das Tool zur Überprüfung der Synchronisierung auszuführen, um sicherzustellen, dass die [!DNL Microsoft Dynamics]-Synchronisierung mit Marketo korrekt eingerichtet ist, bevor Sie die endgültige Verbindung zwischen ihnen herstellen. Der Prozess generiert eine Checkliste mit sieben Einrichtungsschritten, die identifizieren, wo Probleme vorliegen. Wenn Sie überprüfen, ob diese korrekt durchgeführt wurden, können Sie später viel Zeit sparen.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Admin“ und dann auf den Link **[!DNL Microsoft Dynamics]** im Bereich Integration .

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Wählen Sie **[!DNL Microsoft]** aus.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte Synchronisierungseinstellungen]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Geben Sie Ihren Benutzernamen, Ihr Kennwort und Ihre URL ein (Client-ID und Client-Geheimnis sind optional). Klicken Sie abschließend **[!UICONTROL Weiter]**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Wenn Sie zuvor bereits eine Synchronisierung durchgeführt haben **liest** CRM) in der linken Struktur **[!DNL Microsoft Dynamics]** und die Daten im obigen Formular können vorab ausgefüllt werden.

1. Wenn alles in Ordnung ist, generiert die Überprüfungssynchronisierung eine Checkliste voller grüner Auswahlfelder ![ - ](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Wenn ein ![ angezeigt wird - ](assets/delete.png), weist dieser Schritt ein Problem auf. Siehe [Beheben von  [!DNL Dynamics] -Überprüfungsproblemen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md), um das Problem zu identifizieren und zu beheben. Führen Sie dann die Synchronisierungsvalidierungsschritte erneut aus, bis das Ergebnis wie im Bild oben aussieht.

   >[!CAUTION]
   >
   >Wir unterstützen derzeit keine Sandbox-Aktualisierung für die [!DNL Marketo Dynamics]. Wenn Sie Ihre [!DNL Dynamics] CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie von Ihrem Customer Success Manager.

>[!MORELIKETHIS]
>
>[Beheben  [!DNL Dynamics]  Synchronisierungsproblemen bei der Validierung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
