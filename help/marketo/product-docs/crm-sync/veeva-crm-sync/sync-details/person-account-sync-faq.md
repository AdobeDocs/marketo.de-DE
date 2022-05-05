---
description: Häufig gestellte Fragen zur Benutzerkontensynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Benutzerkontosynchronisierung
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Häufig gestellte Fragen zur Benutzerkontosynchronisierung {#person-account-sync-faq}

Marketo Engage synchronisiert Ihre gesamte Datenbank mit Veeva für den Datensatztyp &quot;Benutzerkonto&quot;. Nach der Synchronisation wartet es 5 Minuten und synchronisiert dann den ganzen Tag und jeden Tag erneut.

Personenkonten können in Veeva entsprechend den Anforderungen Ihrer Organisation eingerichtet werden.

>[!NOTE]
>
>Die Standardkonten von Veeva sind Profis.

**Was ist ein Personenkonto?**

Ein Personenkonto ähnelt dem Kontoobjekt in Veeva CRM sehr. Ein Personenkonto hat jedoch Zugriff auf die Felder des Kontos und der Kontaktfelder.

**Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird?**

Ein Personenkonto wird als Unternehmen und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

**Wie kann ich Geschäftskonten und Personenkonten unterscheiden?**

Verwenden Sie den Filter &quot;Is Person&quot;-Konto in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

**Welches E-Mail-Feld sollte ich für Personenkonten verwenden?**

Es gibt zwei E-Mail-Felder für ein Personenkonto. Verwenden Sie das Feld E-Mail-Adresse in Ihren Formularen (nicht die Personen-E-Mail-Adresse), um sicherzustellen, dass die Deduplizierung von Marketo und andere E-Mail-Verarbeitungen ordnungsgemäß funktionieren.

## Synchronisierungsrichtung {#sync-direction}

Die Synchronisation der mit dem Kontakt verbundenen Felder des Personenkontos erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Veeva CRM oder Marketo vornehmen, spiegeln sich Ihre Aktualisierungen in beiden Systemen wider. Die Felder des Kontos werden nur in eine Richtung synchronisiert, von VEeva CRM zu Marketo.

**Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an Kontaktfeldern im Personenkonto vorgenommen werden?**

Wir wären nett und ließen Veeva CRM gewinnen. Es ist jedoch selten, dass diese Art von Datenkollision auftritt.

**Werden Lead- oder Kontakttyp von Datensätzen mit Vevar CRM synchronisiert?**

Veeva CRM behandelt ausschließlich Personen-Account-Objekte und hat auch Geschäftskonten. Die traditionellen CRM-Typen von Lead, Kontakten und Chancen sind in den traditionellen Veeva CRM-Systemen nicht wirklich im Einsatz. Diese können im VEE-CRM erstellt werden und die Synchronisation kann sie in Marketo bringen, sie werden jedoch von diesem Connector nicht offiziell unterstützt.

**Kann ich eine Person in einen Kontakt in Marketo umwandeln?**

Nein, da Lead und Kontakt keine Typen für die Synchronisation mit Veeva CRM unterstützen. Daher wird die Konvertierung nicht unterstützt.

**Kann ich die Synchronisierung eines Kontakts manuell erzwingen?**

Nein, da Kontakt kein unabhängiger Datensatz ist, wird die Synchronisierung einer Person mit Veeva nicht unterstützt.

**Synchronisiert jedes Standardfeld mit Marketo?**

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo Sync User Zugriff hat.

**Wird Marketo die Validierungsregeln von Veeva einhalten?**

Ja, wenn ein Konflikt vorliegt, protokollieren wir das Ergebnis im Aktivitätsprotokoll des Leads.

>[!MORELIKETHIS]
>
>* [Standardmäßige VEA-Feldzuordnung](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [Synchronisieren von Aufrufen und Aufrufen von Schlüsselmeldungen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

