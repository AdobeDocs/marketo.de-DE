---
unique-page-id: 8783322
description: Überprüfen der Microsoft Dynamics-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Überprüfen der Synchronisierung mit Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Überprüfen der Synchronisierung mit Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Wenn Sie die Multi-Factor-Authentifizierung (MFA) für Ihre Dynamics Sync aktiviert haben, müssen Sie sie deaktivieren, damit Dynamics ordnungsgemäß mit Marketo synchronisiert werden kann. Für weitere Informationen wenden Sie sich bitte an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

## Ausführen der Überprüfungssynchronisierung in Marketo {#run-validate-sync-in-marketo}

Es ist sehr wichtig, das Tool zur Validierungssynchronisierung auszuführen, um sicherzustellen, dass die Microsoft Dynamics-Synchronisierung mit Marketo korrekt eingerichtet ist, bevor die endgültige Verbindung hergestellt wird. Der Prozess generiert eine Checkliste mit sieben Einrichtungsschritten, die bestimmen, wo Probleme auftreten. Die Überprüfung dieser Schritte kann später viel Zeit sparen.

1. Klicken Sie auf **[!UICONTROL Admin]** und dann die **[!DNL Microsoft Dynamics]** im Bereich &quot;Integration&quot;.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Auswählen **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Klicken Sie auf **[!UICONTROL Überprüfen der Synchronisierungseinrichtung]** Registerkarte.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Geben Sie Ihren Benutzernamen, Ihr Kennwort und Ihre URL ein (Client-ID und Client-Geheimnis sind optional). Klicks **[!UICONTROL Nächste]** wann geschehen.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Wenn Sie bereits synchronisiert haben, **[!UICONTROL CRM]** im linken Baum wird **[!DNL Microsoft Dynamics]**, und die Daten im obigen Formular können vorausgefüllt werden.

1. Wenn alles in Ordnung ist, generiert die Überprüfungssynchronisierung eine Checkliste mit grünen Häkchen ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Wenn eine ![—](assets/delete.png), weist dieser Schritt ein Problem auf. Siehe [Synchronisierungsprobleme bei der Dynamics-Überprüfung beheben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} , um das Problem zu identifizieren und zu beheben. Führen Sie dann die Synchronisierungs-Validierungsschritte erneut aus, bis das Ergebnis wie das Bild oben aussieht.

   >[!CAUTION]
   >
   >Sandbox-Aktualisierung für Marketo Dynamics Sync wird derzeit nicht unterstützt. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

>[!MORELIKETHIS]
>
>[Synchronisierungsprobleme bei der Dynamics-Überprüfung beheben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
