---
unique-page-id: 2360370
description: Übereinstimmungen mit Programm- und Salesforce-Kampagnen-Status vor der Synchronisierung - Marketo Docs - Produktdokumentation
title: Übereinstimmungen mit Programm-Status und Salesforce-Kampagnen vor der Synchronisierung
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Übereinstimmungen mit den Status von Programmen und Salesforce-Kampagnen vor der Synchronisierung{#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

In diesem Artikel wird beschrieben, wie Sie einen inkompatiblen Statusfehler und Zuordnungsstatus vor der Synchronisierung von Marketo Programm- und Salesforce-Kampagnen beheben.

## Was tun Sie, wenn Sie eine Fehlermeldung {#what-do-you-do-if-you-received-an-error-message} erhalten haben?

Wenn Sie versuchen, eine Synchronisierung mit einer vorhandenen Salesforce-Kampagne durchzuführen, die Interessenten enthält und die Kampagne einen oder mehrere inkompatible Status enthält, wird eine Fehlermeldung angezeigt. Ein Marketo-Programm und eine Salesforce-Kampagne *werden nicht* synchronisiert, wenn die Statusangaben nicht exakt übereinstimmen.

![](assets/image2015-7-22-9-3a23-3a29.png)

In dieser Fehlermeldung können Sie folgende Optionen auswählen:

1. Wählen Sie eine andere Kampagne aus dem Dropdown-Menü ODER
1. Sie können das Problem abbrechen, Statusfehler beheben und nach der Behebung der Fehler eine Synchronisierung durchführen. Führen Sie einen der folgenden Schritte aus, um Statusfehler zu beheben:

   * Melden Sie sich bei Salesforce an und entfernen oder benennen Sie die inkompatiblen Kampagnen-Mitgliedsstaaten um, um den Marketo-Programm-Statusangaben zuzuordnen, die für den mit Ihrem Marketo-Programm verknüpften Kanal verwendet werden.
   * Ändern Sie die Statusangaben des Programms in Marketo, um sie den Mitgliedstaaten der Salesforce-Kampagne zuzuordnen, die Sie eingerichtet haben. Dies ist eine Marketo Admin-Funktion. Weitere Informationen finden Sie unter [Erstellen eines Programm-Kanals](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
