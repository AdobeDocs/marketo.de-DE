---
description: Erfahren Sie, wie Sie die Dynamic Chat-Sicherheit mit blockierten oder zulässigen Domains konfigurieren. Beschränken Sie, welche E-Mail-Domains Agenten sehen und welche Websites Ihr Chatskript verwenden dürfen.
title: Sicherheitseinstellungen
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: 'https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%
---
# Sicherheitseinstellungen {#security-settings}

In den Sicherheitseinstellungen können Sie einer blockierten oder -Zulassungsliste Domains hinzufügen.

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>Die Filterung E-Mail-Domain blockieren und zulassen gilt nur, wenn ein Besucher seine E-Mail-Adresse direkt in Dynamic Chat eingibt, entweder im Chat-Bot oder im Gesprächsfluss. Sie gilt nicht für E-Mail-Adressen, die Dynamic Chat von integrierten Produkten wie Marketo Engage erhält. Weitere Informationen finden Sie in der folgenden Tabelle.

| Szenario | Gilt die Filterung? |
|---|---|
| Der Besucher gibt seine E-Mail-Adresse direkt in den Dynamic Chat-Chatbot ein | Ja |
| Besucher geben ihre E-Mail direkt in einen Dynamic Chat-Gesprächsfluss ein | Ja |
| Die E-Mail wird vorab aus einer Marketo-Formularübermittlung ausgefüllt (der Konversionsfluss wird nach dem Ausfüllen des Formulars angezeigt) | Nein |
| E-Mail wird von jedem anderen integrierten System an Dynamic Chat übergeben | Nein |

## Blockierte E-Mail-Domains {#blocked-email-domains}

Wenn es Besucher mit E-Mail-Domains gibt, mit denen Ihre Agenten nicht interagieren sollen (z. B. ein Wettbewerber), fügen Sie der Blockierungsliste ihre E-Mail-Domain hinzu.

1. Wählen Sie den **Validierung aktivieren**, um Ihre Blockierungsliste zu aktivieren. Geben Sie bis zu 50 Domains ein und klicken Sie auf **Speichern**.

   ![](assets/security-settings-2.png)

## Zulässige Domains {#allowed-domains}

Durch das Hinzufügen von zulässigen Domains wird sichergestellt, dass Dritte das JavaScript nicht von Ihrer Site abschöpfen und zu ihren eigenen hinzufügen können.

1. Wählen Sie den **Validierung aktivieren**, um Ihre Zulassungsliste zu aktivieren. Geben Sie die zulässigen Domains ein und klicken Sie auf **Speichern**.

   ![](assets/security-settings-3.png)
