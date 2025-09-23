---
unique-page-id: 4719316
description: Verwenden von Personenkonten - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Personenkonten
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 2%

---

# Verwenden von Personenkonten {#using-person-accounts}

Personenkonten können in Salesforce entsprechend den Anforderungen Ihres Unternehmens eingerichtet werden. So behandelt Marketo Engage Personenkonten.

>[!NOTE]
>
>Die standardmäßigen [!DNL Salesforce] sind Geschäftskonten. Ihr [!DNL Salesforce]-Administrator muss Personenkonten separat einrichten.

## Was ist ein Personenkonto? {#what-is-a-person-account}

Ein Personenkonto ähnelt dem Kontoobjekt in [!DNL Salesforce]. Ein Personenkonto hat jedoch Zugriff sowohl auf Kontofelder als auch auf Kontaktfelder.

## Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ein Personenkonto wird als Firma und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

## Wie unterscheide ich zwischen Geschäftskonten und Personenkonten? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Verwenden Sie den Filter „Ist-Personen-Konto“ in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

## Wo werden die Informationen zu meinen Personenkonten in Marketo Sales Insight angezeigt? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktivitäten, die sich auf Personenkonten beziehen, werden im Bedienfeld **[!UICONTROL Konto]** angezeigt.

>[!NOTE]
>
>Die Optionen **[!UICONTROL Zu Marketo-Kampagne hinzufügen]** und **[!UICONTROL E-Mail senden]** von Marketo Sales Insight sind derzeit nicht für Personenkonten verfügbar.

## Wie kann ich Opportunities mit einem Personenkonto verknüpfen? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo hängt von der Rolle des Opportunity-Kontakts ab, um zu bestimmen, mit welcher Person die Opportunity verknüpft werden soll. Sie müssen für jedes Personenkonto die Rolle Opportunity-Kontakt hinzufügen, um die Opportunity mit der entsprechenden Person in Marketo zu verbinden. Es wird empfohlen, einen Workflow einzurichten, um die Rolle Opportunity-Kontakt automatisch hinzuzufügen.

## Welches E-Mail-Feld sollte ich für Personenkonten verwenden? {#which-email-field-should-i-use-for-person-accounts}

Für ein Personenkonto gibt es zwei E-Mail-Felder. Verwenden Sie das Feld **[!UICONTROL E-Mail]** in Ihren Formularen (nicht die **[!UICONTROL Personen-E-Mail-Adresse]**), um sicherzustellen, dass die Deduplizierung und andere E-Mail-Verarbeitungen von Marketo ordnungsgemäß funktionieren.
