---
description: Überblick über Adobe Identity Management für Marketo Engage, einschließlich Migrationszeitpunkt, Admin Console-Benutzerverwaltung und Profilebenen wie Systemadministrator und Produktadministrator.
title: Überblick über Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 6%

---

# Überblick über Adobe Identity Management {#adobe-identity-management-overview}

Alle neuen Adobe Marketo Engage-Abonnements (31. Juli 2023 oder höher) sind mit dem Adobe Identity Management-System integriert.

Für Abonnements, die in Adobe Identity integriert sind, wird die Adobe Admin Console für die Benutzerverwaltung verwendet. Identitätsbezogene Konzepte, wie Single Sign-On, werden ebenfalls in der Admin Console verwaltet.

* Weitere Informationen über die [Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}.
* Weitere Informationen zum [Einrichten der Adobe-Organisation im Zusammenhang mit Ihrem Marketo-Abonnement](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Wenn Sie Single Sign-On implementieren möchten und Ihr Abonnement in Adobe Identity integriert wurde, ohne dass SSO in der Adobe-Organisation implementiert ist, senden Sie ein Ticket an den [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie das Thema als &quot;Marketo auf Admin Console, Implementierung von SSO“ an.

## Profilebenen {#profile-levels}

In das Adobe Identity Management-System integrierte Adobe Marketo Engage-Abonnements unterstützen verschiedene Profile. Im Folgenden finden Sie die Typen von Benutzerprofilen, die für diese Integration relevant sind.

<table>
 <tr>
  <td><strong>Adobe Admin Console-Systemadministrator</strong></td>
  <td>Zuständig für die Einrichtung von Identitätskonzepten für die Adobe-Organisation und das Marketo Engage-Produkt in der Adobe Admin Console. Rolle bei der Einrichtung der Adobe-Organisation zugewiesen.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console-Produktadministrator</strong></td>
  <td>Zuständig für die Berechtigung von Benutzern für das Marketo Engage-Produkt in der Adobe Admin Console. Rolle in Adobe Admin Console zugewiesen.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console-Produktprofil-Admin</strong></td>
  <td>Verantwortlich für die Verwaltung von Benutzern innerhalb eines Produktprofils. Sie können keine Benutzer außerhalb dieses spezifischen Profils verwalten. Ein Produktprofil-Administrator bzw. eine Produktprofil-Administratorin hat keinen Zugriff auf das Marketo-Programm, es sei denn, er bzw. sie wird dem Produktprofil als Benutzende hinzugefügt. Ihre Rolle wäre weiterhin ein Standardbenutzer (Standardarbeitsbereich, wenn mehrere Arbeitsbereiche vorhanden sind).
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage Admin</strong></td>
  <td>Eine Person, die Zugriff auf Marketo Engage mit Administratorrechten erhalten hat. Zugewiesene Rolle in Marketo Engage, nicht in Adobe Admin Console (wird nur als „Admin“ im Modal <b>Benutzer bearbeiten</b> angezeigt).</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage-Benutzer</strong></td>
  <td>Eine Person, die Zugriff auf Marketo Engage erhalten hat. Keine Administratorrechte.</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [Admin-Setup](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Hinzufügen oder Entfernen eines Produktadministrators](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [Benutzer hinzufügen oder entfernen](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
