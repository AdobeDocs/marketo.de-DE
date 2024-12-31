---
description: Häufig gestellte Fragen zur Synchronisierung von Benutzerkonten - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Synchronisierung von Personenkonten
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Häufig gestellte Fragen zur Synchronisierung von Personenkonten {#person-account-sync-faq}

Marketo Engage synchronisiert Ihre gesamte Datenbank mit Veeva nach dem Datensatztyp des Personenkontos. Nach der Synchronisierung wartet er 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag.

Personenkonten können in Veeva entsprechend den Anforderungen Ihres Unternehmens eingerichtet werden.

>[!NOTE]
>
>Wir synchronisieren nur „Professional“-Stufen-Konten als Personenkonten.

**Was ist ein Personenkonto?**

Ein Personenkonto ist dem Kontoobjekt in Veeva CRM sehr ähnlich. Ein Personenkonto hat jedoch Zugriff sowohl auf Kontofelder als auch auf Kontaktfelder.

**Was passiert, wenn ein Personenkonto mit Marketo synchronisiert wird?**

Ein Personenkonto wird als Firma und als Person mit Marketo synchronisiert.

>[!NOTE]
>
>Die benutzerdefinierten Felder für ein Personenkonto werden sowohl in das Unternehmen als auch in die Person in Marketo kopiert.

**Wie unterscheide ich zwischen Geschäftskonten und Personenkonten?**

Verwenden Sie den Kontofilter „Ist Person“ in Ihrer Smart-Liste, um Personenkonten von standardmäßigen Geschäftskonten zu trennen.

**Welches E-Mail-Feld sollte ich für Personenkonten verwenden?**

Für ein Personenkonto gibt es zwei E-Mail-Felder. Verwenden Sie das Feld E-Mail-Adresse in Ihren Formularen (nicht die E-Mail-Adresse der Person), um sicherzustellen, dass die Deduplizierung und andere E-Mail-Verarbeitungen von Marketo ordnungsgemäß funktionieren.

## Synchronisationsrichtung {#sync-direction}

Die Synchronisierung von kontaktbezogenen Feldern des Personenkontos erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Veeva CRM oder Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt. Die Felder im Konto werden nur in eine Richtung synchronisiert, von Veeva CRM zu Marketo.

**Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an den Feldern „Kontakt“ im Personenkonto vorgenommen werden?**

Wir wären nett und lassen Veeva CRM gewinnen. Es kommt jedoch selten vor, dass solche Datenkollisionen auftreten.

**Sind Datensätze vom Typ Lead oder Kontakt mit dem Veeva CRM synchronisiert?**

Veeva CRM behandelt nur Personenkontoobjekte und verfügt auch über Geschäftskonten. Die traditionellen CRM-Typen Lead, Kontakte und Opportunities werden in traditionellen Veeva-CRM-Systemen nicht wirklich verwendet. Diese können in Veeva CRM erstellt werden, werden jedoch offiziell nicht mit diesem Connector unterstützt.

**Kann ich eine Person in Marketo in einen Kontakt konvertieren?**

Nein, da Lead und Kontakt keine unterstützten Typen für die Synchronisierung mit Veeva CRM sind. Daher wird die Konvertierung nicht unterstützt.

**Kann ich die Synchronisierung eines Kontakts manuell erzwingen?**

Nein, da Kontakt kein unabhängiger Datensatztyp ist, wird das Synchronisieren einer Person mit Veeva nicht unterstützt.

**Wird jedes Standardfeld mit Marketo synchronisiert?**

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo-Synchronisierungsbenutzer Zugriff hat.

**Wird Marketo die Veeva-Validierungsregeln einhalten?**

Ja, wenn ein Konflikt besteht, protokollieren wir das Ergebnis im Aktivitätsprotokoll des Leads.

>[!MORELIKETHIS]
>
>* [Standard-Veeva-Feldzuordnung](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Meldungen zu Aufrufen und Aufrufen synchronisieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
