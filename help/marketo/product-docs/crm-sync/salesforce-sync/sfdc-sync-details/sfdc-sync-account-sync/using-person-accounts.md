---
unique-page-id: 4719316
description: Verwenden von Benutzerkonten - Marketo Docs - Produktdokumentation
title: Verwenden von Benutzerkonten
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
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

## Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ein Personenkonto wird mit Marketo als Firma und als Person synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Benutzerkonto werden sowohl in die Firma als auch in die Person in Marketo kopiert.

## Wie differenziere ich Geschäftskonten und Personenkonten? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Verwenden Sie den Filter **Ist-Personenkonto** in Ihrer intelligenten Liste, um Personenkonten von Standardkonten zu trennen.

## Wo werden die persönlichen Kontoinformationen in Marketo Sales Insight angezeigt? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktivitäten zu Personenkonten werden im Bedienfeld **Konto** angezeigt.

>[!NOTE]
>
>Die Optionen **Hinzufügen an Marketo Kampagne** und **E-Mail senden** von Marketo Sales Insight stehen derzeit nicht für Personenkonten zur Verfügung.

## Wie verknüpfe ich Chancen mit einem Personenkonto? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo hängt von der Kontaktrolle für die Möglichkeit ab, zu bestimmen, welche Person die Gelegenheit erhält. Sie müssen die Kontaktfunktion für die Kontaktaufnahme mit jedem Benutzerkonto hinzufügen, um die Gelegenheit mit der entsprechenden Person in Marketo zu verbinden. Es wird empfohlen, einen Arbeitsablauf einzurichten, um die Kontaktrolle automatisch hinzuzufügen.

## Welches E-Mail-Feld sollte ich für Personenkonten verwenden? {#which-email-field-should-i-use-for-person-accounts}

Es gibt zwei E-Mail-Felder für ein Personenkonto. Verwenden Sie das Feld **E-Mail-Adresse** in Ihren Formularen (nicht **E-Mail-Adresse der Person**), um sicherzustellen, dass die Deduplizierung und andere E-Mail-Verarbeitung von Marketo ordnungsgemäß funktionieren.
