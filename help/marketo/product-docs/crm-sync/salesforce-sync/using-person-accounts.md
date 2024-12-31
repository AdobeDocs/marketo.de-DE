---
unique-page-id: 4719316
description: Verwenden von Personenkonten - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Personenkonten
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Verwenden von Personenkonten {#using-person-accounts}

Personenkonten können in Salesforce entsprechend den Anforderungen Ihres Unternehmens eingerichtet werden. So behandelt Marketo Engage Personenkonten.

>[!NOTE]
>
>Die standardmäßigen Salesforce-Konten sind Geschäftskonten. Ihr Salesforce-Administrator muss Personenkonten separat einrichten.

## Was ist ein Personenkonto? {#what-is-a-person-account}

Ein Personenkonto ähnelt dem Kontoobjekt in Salesforce. Ein Personenkonto hat jedoch Zugriff sowohl auf Kontofelder als auch auf Kontaktfelder.

## Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ein Personenkonto wird als Firma und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

## Wie unterscheide ich zwischen Geschäftskonten und Personenkonten? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Verwenden Sie den Filter „Ist-Personen-Konto“ in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

## Wo werden in Marketo Sales Insight Informationen zu persönlichen Konten angezeigt? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktivitäten, die sich auf Personenkonten beziehen, werden im Bedienfeld **[!UICONTROL Konto]** angezeigt.

>[!NOTE]
>
>Die Optionen **[!UICONTROL Zu Marketo-Kampagne hinzufügen]** und **[!UICONTROL E-Mail]** von Marketo Sales Insight sind derzeit nicht für Personenkonten verfügbar.

## Wie kann ich Opportunities mit einem Personenkonto verknüpfen? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo hängt von der Rolle des Opportunity-Kontakts ab, um zu bestimmen, mit welcher Person die Opportunity verknüpft werden soll. Sie müssen für jedes Personenkonto die Rolle Opportunity-Kontakt hinzufügen, um die Opportunity mit der entsprechenden Person in Marketo zu verbinden. Es wird empfohlen, einen Workflow einzurichten, um die Rolle Opportunity-Kontakt automatisch hinzuzufügen.

## Welches E-Mail-Feld sollte ich für Personenkonten verwenden? {#which-email-field-should-i-use-for-person-accounts}

Für ein Personenkonto gibt es zwei E-Mail-Felder. Verwenden Sie das Feld **E-Mail** in Ihren Formularen (nicht die **Personen-E-Mail-Adresse**), um sicherzustellen, dass die Deduplizierung und andere E-Mail-Verarbeitungen von Marketo ordnungsgemäß funktionieren.
