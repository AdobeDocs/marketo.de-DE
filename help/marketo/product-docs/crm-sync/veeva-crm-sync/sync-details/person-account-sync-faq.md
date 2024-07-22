---
description: Häufig gestellte Fragen zur Benutzerkontensynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Benutzerkontensynchronisierung
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Häufig gestellte Fragen zur Benutzerkontensynchronisierung {#person-account-sync-faq}

Marketo Engage synchronisiert Ihre gesamte Datenbank mit Veeva für den Datensatztyp &quot;Benutzerkonto&quot;. Nach der Synchronisation wartet es 5 Minuten und synchronisiert dann den ganzen Tag und jeden Tag erneut.

Personenkonten können in Veeva entsprechend den Anforderungen Ihrer Organisation eingerichtet werden.

>[!NOTE]
>
>Wir synchronisieren nur &quot;Professional&quot;-Statuskonten als Personenkonten.

**Was ist ein Personenkonto?**

Ein Personenkonto ähnelt dem Kontoobjekt in Veeva CRM sehr. Ein Personenkonto hat jedoch Zugriff auf die Felder des Kontos und der Kontaktfelder.

**Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird?**

Ein Personenkonto wird als Unternehmen und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

**Wie differenziere ich Geschäftskonten und Personenkonten?**

Verwenden Sie den Filter &quot;Is Person&quot;-Konto in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

**Welches E-Mail-Feld sollte ich für Personenkonten verwenden?**

Es gibt zwei E-Mail-Felder für ein Personenkonto. Verwenden Sie das Feld E-Mail-Adresse in Ihren Formularen (nicht die Personen-E-Mail-Adresse), um sicherzustellen, dass die Deduplizierung von Marketo und andere E-Mail-Verarbeitungen ordnungsgemäß funktionieren.

## Synchronisierungsrichtung {#sync-direction}

Die Synchronisation der mit dem Kontakt verbundenen Felder des Personenkontos erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Veeva CRM oder Marketo vornehmen, spiegeln sich Ihre Aktualisierungen in beiden Systemen wider. Die Felder des Kontos werden nur in eine Richtung synchronisiert, von VEeva CRM zu Marketo.

**Was passiert, wenn Änderungen in beiden Systemen gleichzeitig in Kontaktfelder für das Personenkonto vorgenommen werden?**

Wir wären nett und ließen Veeva CRM gewinnen. Es ist jedoch selten, dass diese Art von Datenkollision auftritt.

**Werden Lead- oder Kontakttyp von Datensätzen mit VEeva CRM synchronisiert?**

Veeva CRM behandelt ausschließlich Personen-Account-Objekte und hat auch Geschäftskonten. Die traditionellen CRM-Typen von Lead, Kontakten und Chancen sind in den traditionellen Veeva CRM-Systemen nicht wirklich im Einsatz. Diese können im VEE-CRM erstellt werden, werden jedoch nicht offiziell über diesen Connector unterstützt.

**Kann ich eine Person in einen Kontakt in Marketo umwandeln?**

Nein, da Lead und Kontakt keine Typen für die Synchronisation mit Veeva CRM unterstützen. Daher wird die Konvertierung nicht unterstützt.

**Kann ich die Synchronisierung eines Kontakts manuell erzwingen?**

Nein, da Kontakt kein unabhängiger Datensatz ist, wird die Synchronisierung einer Person mit Veeva nicht unterstützt.

**Synchronisiert jedes Standardfeld mit Marketo?**

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo Sync User Zugriff hat.

**Wird Marketo die VEA-Validierungsregeln einhalten?**

Ja, wenn ein Konflikt vorliegt, protokollieren wir das Ergebnis im Aktivitätsprotokoll des Leads.

>[!MORELIKETHIS]
>
>* [Standardmäßige Visualisierungsfeldzuordnung](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Synchronisierungsaufruf und -aufruf für Schlüsselmeldungen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
