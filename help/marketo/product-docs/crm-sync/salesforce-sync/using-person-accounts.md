---
unique-page-id: 4719316
description: Verwenden von Personenkonten - Marketo Docs - Produktdokumentation
title: Verwenden von Personenkonten
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Verwenden von Personenkonten {#using-person-accounts}

Personenkonten können in Salesforce entsprechend den Anforderungen Ihrer Organisation eingerichtet werden. So behandelt Marketo Personenkonten.

>[!NOTE]
>
>Die Salesforce-Standardkonten sind Geschäftskonten. Ihr Salesforce-Administrator muss Personenkonten separat einrichten.

## Was ist ein Personenkonto? {#what-is-a-person-account}

Ein Personenkonto ähnelt dem Kontoobjekt in Salesforce sehr. Ein Personenkonto hat jedoch Zugriff auf die Felder des Kontos und der Kontaktfelder.

## Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ein Personenkonto wird als Unternehmen und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

## Wie kann ich Geschäftskonten und Personenkonten unterscheiden? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Verwenden Sie den Filter **Is Person Account** in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

## Wo werden die Informationen zu meinen Personenkonten in Marketo Sales Insight angezeigt? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktivitäten im Zusammenhang mit Personenkonten werden im Bereich **Konto** angezeigt.

>[!NOTE]
>
>Die Optionen **Zu Marketo Campaign hinzufügen** und **E-Mail senden** von Marketo Sales Insight stehen derzeit nicht für Personenkonten zur Verfügung.

## Wie ordne ich einem Personenkonto Chancen zu? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo hängt von der Rolle des Opportunity-Kontakts ab, um zu bestimmen, welcher Person die Möglichkeit zugeordnet werden soll. Sie müssen für jedes Personenkonto die Kontaktrolle hinzufügen, um die Möglichkeit mit der entsprechenden Person in Marketo zu verbinden. Es wird empfohlen, einen Workflow einzurichten, um die Rolle &quot;Opportunity Contact&quot;automatisch hinzuzufügen.

## Welches E-Mail-Feld sollte ich für Personenkonten verwenden? {#which-email-field-should-i-use-for-person-accounts}

Es gibt zwei E-Mail-Felder für ein Personenkonto. Verwenden Sie das Feld **E-Mail-Adresse** in Ihren Formularen (nicht das Feld **Personen-E-Mail-Adresse**), um sicherzustellen, dass die Deduplizierung von Marketo und andere E-Mail-Verarbeitungen ordnungsgemäß funktionieren.