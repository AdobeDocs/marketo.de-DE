---
unique-page-id: 37357050
description: Aktualisieren des MSI-Pakets - Marketo-Dokumente - Produktdokumentation
title: Aktualisieren des MSI-Pakets
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 3%

---

# Aktualisieren des MSI-Pakets {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>Aufgrund der von Salesforce vorgenommenen Sicherheitsverbesserungen kann das Insight-Verkaufspaket keine Berechtigung mehr für Standardobjekte gewähren. Künftig benötigt das Salesforce-Profil von Sales Insight-Benutzenden Lesezugriff auf die folgenden Standardobjekte: Lead, Kontakt, Konto und Opportunity. [Hier erfahren Sie, wie Sie dies konfigurieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Navigieren Sie zu [dieser Seite in der AppExchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Melden Sie sich bei Ihrer [!DNL Salesforce]-Instanz (die mit Ihrer Marketo-Instanz verbunden ist, kann Sandbox oder Produktion sein) oben rechts auf der Seite in Schritt 1 an. Sie müssen über Administratorrechte verfügen, um ein verwaltetes Paket in [!DNL Salesforce] zu installieren/aktualisieren.

1. Klicken Sie auf **Schaltfläche „Jetzt abrufen**. Sie werden aufgefordert, den Ort auszuwählen, an dem Sie installieren möchten. Sie erhalten die Möglichkeit, ein Upgrade durchzuführen, da Sie bereits über eine frühere Version von MSI verfügen. Wählen Sie eine Option basierend auf dem Konto aus, bei dem Sie sich in Schritt 1 angemeldet haben.

   >[!TIP]
   >
   >Es wird empfohlen, dies auf Ihrer Sandbox-Instanz zu testen, bevor Sie ein Upgrade Ihrer Produktionsinstanz durchführen.

1. Sie können das Paket aktualisieren, indem Sie „Nur für Administratoren installieren“ (und später MSI-Zugriff auf bestimmte Profile gewähren), „Für alle Benutzer installieren“ oder „Für bestimmte Profile installieren“ auswählen. In diesem Beispiel wählen wir „Nur Administratoren“. Wenn Sie Ihre Auswahl getroffen haben, klicken Sie auf **Upgrade**.

   ![](assets/four.png)

>[!NOTE]
>
>Es wird empfohlen, das Paket nur für Administratoren zu aktualisieren und dann [bestimmten Benutzern Zugriff zu gewähren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} basierend auf der Anzahl der erworbenen MSI-Lizenzen. Alternativ können Sie ein bestimmtes Salesforce-Profil für MSI-Benutzer erstellen und das Paket nur für diese Benutzer installieren oder aktualisieren.
