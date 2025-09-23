---
unique-page-id: 2360370
description: Programmstatus und Salesforce-Kampagnenstatus vor der Synchronisierung abgleichen - Marketo-Dokumente - Produktdokumentation
title: Wie sich Programmstatus und Salesforce-Kampagnenstatus vor der Synchronisierung abgleichen lassen
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 5%

---

# Programmstatus und [!DNL Salesforce] Kampagnenstatus vor der Synchronisierung abgleichen {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

In diesem Artikel wird beschrieben, wie Sie einen inkompatiblen Statusfehler beheben und Status vor der Synchronisierung von Marketo-Programmen und [!DNL Salesforce] Campaign zuordnen können.

## Was tun, wenn Sie eine Fehlermeldung erhalten haben {#what-do-you-do-if-you-received-an-error-message}

Wenn Sie versuchen, eine Synchronisierung mit einer vorhandenen [!DNL Salesforce]-Kampagne durchzuführen, die Leads enthält und die Kampagne einen oder mehrere inkompatible Status aufweist, wird eine Fehlermeldung angezeigt. Ein Marketo-Programm und eine [!DNL Salesforce]-*werden nicht synchronisiert* wenn die Status nicht exakt übereinstimmen.

![](assets/image2015-7-22-9-3a23-3a29.png)

Bei dieser Fehlermeldung haben Sie folgende Möglichkeiten:

1. Wählen Sie im Dropdown-Menü eine andere Kampagne aus, mit der synchronisiert werden soll, ODER
1. Sie können den Vorgang abbrechen, die Statusfehler beheben und versuchen, nach Behebung der Fehler zu synchronisieren. Führen Sie einen der folgenden Schritte aus, um die Statusfehler zu beheben:

   * Melden Sie sich bei Salesforce an und entfernen Sie die inkompatiblen Campaign-Mitgliedsstatus oder benennen Sie sie um, um sie den Marketo-Programmstatus zuzuordnen, die für den mit Ihrem Marketo-Programm verknüpften Kanaltyp verwendet werden.
   * Ändern Sie den Programmstatus in Marketo, um ihn den bestehenden Salesforce Campaign-Mitgliedsstatus zuzuordnen. Dies ist eine Marketo Admin-Funktion. Weitere Informationen finden Sie unter [Erstellen eines Programmkanals](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
