---
unique-page-id: 37357050
description: Aktualisieren Ihres MSI-Pakets - Marketo-Dokumente - Produktdokumentation
title: Upgrade Ihres MSI-Pakets
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: ddc9242bdf1b3ec34bb2672821b6b054647d94b5
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Upgrade Ihres MSI-Pakets {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>Aufgrund der von Salesforce vorgenommenen Sicherheitsverbesserungen kann das Sales Insight-Paket keine Berechtigung mehr für Standardobjekte erteilen. Zukünftig muss das Salesforce-Profil von Sales Insight-Benutzern Lesezugriff auf die folgenden Standardobjekte haben: Lead, Kontakt, Konto und Opportunity. [Hier erfahren Sie, wie Sie das konfigurieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Navigieren Sie zu [diese Seite im Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Melden Sie sich oben rechts auf der Seite von Schritt 1 bei Ihrer Salesforce-Instanz an (die mit Ihrer Marketo-Instanz verbunden ist und Sandbox oder Produktion sein kann). Sie müssen über Administratorrechte verfügen, um ein verwaltetes Paket in Salesforce installieren/aktualisieren zu können.

1. Klicken Sie auf **Jetzt downloaden** Schaltfläche. Sie werden gebeten zu wählen, wo Sie installieren möchten. Sie erhalten die Möglichkeit, ein Upgrade durchzuführen, da Sie bereits über eine frühere Version von MSI verfügen. Wählen Sie eine Option basierend auf dem Konto, bei dem Sie sich während Schritt 1 angemeldet haben.

   >[!TIP]
   >
   >Es wird empfohlen, dies auf Ihrer Sandbox-Instanz zu testen, bevor Sie Ihre Produktionsinstanz aktualisieren.

1. Sie können das Paket aktualisieren, indem Sie &quot;Nur für Administratoren installieren&quot;(und später MSI-Zugriff auf bestimmte Profile gewähren), &quot;Für alle Benutzer installieren&quot;oder &quot;Für bestimmte Profile installieren&quot;auswählen. In diesem Beispiel wählen wir &quot;Nur Administratoren&quot;. Klicken Sie nach Auswahl auf **Upgrade**.

   ![](assets/four.png)

>[!NOTE]
>
>Es wird empfohlen, das Paket nur für Administratoren zu aktualisieren und dann [Zugriff auf bestimmte Benutzer gewähren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} basierend auf der Anzahl der erworbenen MSI-Sitze. Alternativ können Sie ein bestimmtes Salesforce-Profil für MSI-Benutzer erstellen und das Paket nur für diese Benutzer installieren oder aktualisieren.
