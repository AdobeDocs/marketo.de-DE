---
unique-page-id: 4719316
description: Verwenden von Benutzerkonten - Marketing Docs - Produktdokumentation
title: Verwenden von Benutzerkonten
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Verwenden von Personenkonten {#using-person-accounts}

Personenkonten können in Salesforce eingerichtet werden, um den Anforderungen Ihres Unternehmens gerecht zu werden. So behandelt Marketo Personenkonten.

>[!NOTE]
>
>Die Salesforce-Standardkonten sind Geschäftskonten. Ihr Salesforce-Administrator muss Personenkonten separat einrichten.

## Was ist ein Personenkonto? {#what-is-a-person-account}

Ein Personenkonto ist dem Kontoobjekt in Salesforce sehr ähnlich. Ein Benutzerkonto hat jedoch Zugriff sowohl auf die Kontofelder als auch auf die Kontaktfelder.

## Was passiert, wenn ein Benutzerkonto mit Marketo synchronisiert wird? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ein Personenkonto wird mit Marketo als Firma und als Person synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Benutzerkonto werden sowohl in die Firma als auch in die Person in Marketo kopiert.

## Wie differenziere ich Geschäftskonten und Personenkonten? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Verwenden Sie den Filter **Ist-Personenkonto** in Ihrer intelligenten Liste, um Personenkonten von Standardkonten zu trennen.

## Wo werden die Daten meiner persönlichen Konten in Marketo Sales Insight angezeigt? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktivitäten zu Personenkonten werden im Bedienfeld **Konto** angezeigt.

>[!NOTE]
>
>Marketo Sales Insight&#39;s **Hinzufügen an Marketing Kampagne **und **E-Mail senden **Optionen sind derzeit nicht für Personenkonten verfügbar.

## Wie verknüpfe ich Chancen mit einem Personenkonto? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo hängt von der Möglichkeit der Kontaktrolle ab, um zu bestimmen, welche Person die Gelegenheit zu verbinden. Sie müssen die Kontaktrolle für die Möglichkeit jedes persönlichen Kontos hinzufügen, um die Gelegenheit mit der entsprechenden Person in Marketo zu verbinden. Es wird empfohlen, einen Arbeitsablauf einzurichten, um die Kontaktrolle automatisch hinzuzufügen.

## Welches E-Mail-Feld sollte ich für Personenkonten verwenden? {#which-email-field-should-i-use-for-person-accounts}

Es gibt zwei E-Mail-Felder für ein Personenkonto. Verwenden Sie das Feld **E-Mail-Adresse** in Ihren Formularen (nicht **E-Mail-Adresse der Person**), um sicherzustellen, dass die Deduplizierung und andere E-Mail-Verarbeitung von Marketo ordnungsgemäß funktionieren.
