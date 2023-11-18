---
description: Dynamics-Authentifizierungsmethode neu konfigurieren - Marketo Docs - Produktdokumentation
title: Authentifizierungsmethode für Dynamics neu konfigurieren
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Authentifizierungsmethode für Dynamics neu konfigurieren {#reconfigure-dynamics-authentication-method}

Gehen Sie wie folgt vor, um Ihre Dynamics-Authentifizierungsmethode zu aktualisieren.

>[!PREREQUISITES]
>
>Richten Sie die Anwendung in Microsoft Dynamics und das aktive Verzeichnis (Azure AD/ADFS) mithilfe der gewünschten Authentifizierungsmethode aus einem der folgenden Artikel ein:
>
>* [Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Klicken Sie unter Marketo Engage auf **[!UICONTROL Admin]**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Klicks **[!DNL Microsoft Dynamics]**, dann **[!UICONTROL Synchronisierung deaktivieren]**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um die Authentifizierungsmethode zu aktualisieren.

1. Klicken Sie auf **[!UICONTROL Neue Authentifizierungsmethode neu konfigurieren]** Registerkarte.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Wählen Sie die gewünschte neue Authentifizierungsmethode aus (in diesem Beispiel wählen wir die Web-API aus).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Geben Sie die für die neue Authentifizierungsmethode erforderlichen Anmeldeinformationen ein und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Die spezifischen Felder variieren je nach gewählter Authentifizierungsmethode und das Formular wird automatisch je nach vorheriger Authentifizierungsmethode aktualisiert.
   >* Wenn Sie bereits eine Synchronisierung durchgeführt haben, werden die Daten im obigen Formular möglicherweise vorab ausgefüllt. Bitte geben Sie alle Anmeldedaten erneut ein, um die korrekten Werte sicherzustellen.

1. Wenn alles in Ordnung ist, werden bei der Überprüfung der Synchronisierung alle grünen Häkchen generiert ![](assets/green-check.png). Überprüfen Sie die Nachricht und klicken Sie auf **[!UICONTROL Switch]** , um die Authentifizierungsmethode zu aktualisieren.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Wenn eine ![](assets/red-x.png), weist dieser Schritt ein Problem auf. Siehe [Synchronisierungsprobleme bei der Dynamics-Überprüfung beheben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} zur Identifizierung und Behebung des Problems/der Probleme. Führen Sie dann die Synchronisierungs-Validierungsschritte erneut aus, bis das Ergebnis wie das Bild oben aussieht.

1. Klicks **[!UICONTROL Bestätigen]** um fortzufahren.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Klicks **[!UICONTROL Bestätigen]** erneut.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Klicks **[!UICONTROL OK]**.

   >[!IMPORTANT]
   >
   >Es dauert 15 Minuten, bis das System den neuen Authentifizierungsmodus akzeptiert. Warten Sie 15 Minuten ab dem Zeitpunkt des Switches, bevor Sie die Synchronisierung erneut aktivieren.
