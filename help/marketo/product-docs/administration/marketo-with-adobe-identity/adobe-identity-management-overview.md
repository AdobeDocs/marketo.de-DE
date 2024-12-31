---
description: Adobe Identity Management - Übersicht - Marketo-Dokumente - Produktdokumentation
title: Adobe Identity Management - Überblick
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 8d4a542687119e7e4044b26eeafcc71315609f19
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Adobe Identity Management - Überblick {#adobe-identity-management-overview}

Alle neuen Adobe Marketo Engage-Abonnements (31. Juli 2023 oder höher) sind mit dem Adobe Identity Management-System integriert. Bestehende Marketo Engage-Abonnements werden derzeit bei jedem Verkaufsereignis, einschließlich Verlängerungen, Neuverträgen und/oder Addendums, in das Adobe Identity Management-System migriert. Migrationen außerhalb eines Verkaufsereignisses werden ab Oktober 2024 unterstützt. Marketo-Administratoren erhalten 2-4 Wochen im Voraus eine Benachrichtigung, wenn ihr Abonnement außerhalb eines Verkaufsereignisses migriert werden soll.

>[!NOTE]
>
>Der Marketo-Support kann keine Aktualisierungen zur Adobe IMS-Migration bereitstellen. Das Adobe-Account-Team wird sich in den nächsten Monaten mit dem voraussichtlichen Zeitplan in Verbindung setzen. Weitere Informationen finden Sie [diesem Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} und in den [Häufig gestellte Fragen](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Für Abonnements, die auf Adobe-Identitäten integriert wurden, wird die Adobe Admin Console für die Benutzerverwaltung verwendet. Identitätsbezogene Konzepte, wie Single Sign-On, werden ebenfalls in der Admin Console verwaltet.

* Weitere Informationen über die [Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}.
* Weitere Informationen zum [Einrichten der Adobe-Organisation im Zusammenhang mit Ihrem Marketo-Abonnement](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Wenn Sie Single Sign-On implementieren möchten und Ihr Abonnement auf Adobe Identity integriert wurde, ohne dass SSO in der Adobe-Organisation implementiert ist, senden Sie ein Ticket an den [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie das Thema als &quot;Marketo bei Admin Console, SSO implementieren“ an.

## Profilebenen {#profile-levels}

Auf dem Adobe-Identity Management-System integrierte Adobe Marketo Engage-Abonnements unterstützen verschiedene Profile. Im Folgenden finden Sie die Typen von Benutzerprofilen, die für diese Integration relevant sind.

<table>
 <tr>
  <td><strong>Adobe Admin Console-Systemadministrator</strong></td>
  <td>Verantwortlich für die Einrichtung von Identitätskonzepten für die Adobe-Organisation und das Marketo Engage-Produkt in der Adobe Admin Console. Rolle bei der Einrichtung der Adobe-Organisation zugewiesen.</td>
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
  <td><strong>Marketo Engage-Administrator</strong></td>
  <td>Eine Person, die Zugriff auf Marketo Engage mit Administratorrechten erhalten hat. Rolle auf dem Marketo Engage zugewiesen, nicht auf Adobe Admin Console (wird im Modal <b>Benutzer bearbeiten</b> nur als „Admin“ angezeigt).</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage-Benutzer</strong></td>
  <td>Eine Person, die Zugriff auf Marketo Engage erhalten hat. Keine Administratorrechte.</td>
 </tr>
</table>

## FAQs {#faq}

Häufig gestellte Fragen [finden Sie hier](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Admin-Setup](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Hinzufügen oder Entfernen eines Produktadministrators](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Benutzer hinzufügen oder entfernen](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
