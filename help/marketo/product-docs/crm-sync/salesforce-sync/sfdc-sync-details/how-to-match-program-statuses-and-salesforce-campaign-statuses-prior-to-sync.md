---
unique-page-id: 2360370
description: Abgleichen von Programmstatus und Salesforce-Kampagnenstatus vor der Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Abgleichen von Programmstatus und Salesforce-Kampagnenstatus vor der Synchronisierung
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Abgleichen von Programmstatus und Salesforce-Kampagnenstatus vor der Synchronisierung {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

In diesem Artikel wird beschrieben, wie Sie einen inkompatiblen Statusfehler beheben und Status vor der Synchronisierung mit dem Marketo-Programm und Salesforce-Kampagnen zuordnen.

## Was tun Sie, wenn Sie eine Fehlermeldung erhalten? {#what-do-you-do-if-you-received-an-error-message}

Wenn Sie versuchen, eine Synchronisation mit einer vorhandenen Salesforce-Kampagne durchzuführen, die Leads enthält und die Kampagne einen oder mehrere inkompatible Status enthält, wird eine Fehlermeldung angezeigt. Ein Marketo-Programm und eine Salesforce-Kampagne *werden nicht synchronisiert, wenn die Status nicht exakt übereinstimmen.*

![](assets/image2015-7-22-9-3a23-3a29.png)

In dieser Fehlermeldung können Sie Folgendes auswählen:

1. Wählen Sie eine andere Kampagne aus dem Dropdown-Menü aus, mit der synchronisiert werden soll, ODER
1. Sie können eine Fehlerbehebung vornehmen, Statusfehler beheben und versuchen, eine Synchronisierung durchzuführen, sobald die Fehler behoben wurden. Führen Sie einen der folgenden Schritte aus, um die Statusfehler zu beheben:

   * Melden Sie sich bei Salesforce an und entfernen oder benennen Sie die inkompatiblen Campaign-Mitgliedstaaten um, um sie den Marketo-Programmstatus zuzuordnen, die für den mit Ihrem Marketo-Programm verknüpften Kanaltyp verwendet werden.
   * Ändern Sie die Programmstatus in Marketo so, dass sie den vorhandenen Salesforce Campaign-Mitgliedstaaten zugeordnet werden. Dies ist eine Marketo Admin-Funktion. Weitere Informationen finden Sie unter [Erstellen eines Programmkanals](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
