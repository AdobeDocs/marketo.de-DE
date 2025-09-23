---
description: Häufig gestellte Fragen zur Synchronisierung von Benutzerkonten - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zur Synchronisierung von Personenkonten
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Häufig gestellte Fragen zur Synchronisierung von Personenkonten {#person-account-sync-faq}

Marketo Engage synchronisiert Ihre gesamte Datenbank mit [!DNL Veeva] für den Datensatztyp „Personenkonto“. Nach der Synchronisierung wartet er 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag.

Personenkonten können in [!DNL Veeva] eingerichtet werden, um den Anforderungen Ihres Unternehmens zu entsprechen.

>[!NOTE]
>
>Wir synchronisieren nur „Professional“-Stufen-Konten als Personenkonten.

**Was ist ein Personenkonto?**

Ein Personenkonto ähnelt dem Kontoobjekt in [!DNL Veeva] CRM. Ein Personenkonto hat jedoch Zugriff sowohl auf Kontofelder als auch auf Kontaktfelder.

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

Die Synchronisierung von kontaktbezogenen Feldern des Personenkontos erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in [!DNL Veeva] CRM oder Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt. Die Felder im Konto werden nur in eine Richtung synchronisiert, von [!DNL Veeva] CRM zu Marketo.

**Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an den Feldern „Kontakt“ im Personenkonto vorgenommen werden?**

Wir wären nett und lassen [!DNL Veeva] CRM gewinnen. Es kommt jedoch selten vor, dass solche Datenkollisionen auftreten.

**Sind Datensätze vom Typ Lead oder Kontakt mit [!DNL Veeva] CRM synchronisiert?**

[!DNL Veeva] CRM behandelt nur Personenkontoobjekte und verfügt auch über Geschäftskonten. Die herkömmlichen CRM-Typen Lead, Kontakte und Opportunities werden in herkömmlichen [!DNL Veeva]-CRM-Systemen nicht wirklich verwendet. Diese können in [!DNL Veeva] CRM erstellt werden, werden jedoch mit diesem Connector nicht offiziell unterstützt.

**Kann ich eine Person in Marketo in einen Kontakt konvertieren?**

Nein, da Lead und Kontakt keine unterstützten Typen für die Synchronisierung mit [!DNL Veeva] CRM sind. Daher wird die Konvertierung nicht unterstützt.

**Kann ich die Synchronisierung eines Kontakts manuell erzwingen?**

Nein, da der Kontakt kein unabhängiger Datensatztyp ist, wird das Synchronisieren einer Person mit [!DNL Veeva] nicht unterstützt.

**Wird jedes Standardfeld mit Marketo synchronisiert?**

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo-Synchronisierungsbenutzer Zugriff hat.

**Wird Marketo die [!DNL Veeva] Validierungsregeln einhalten?**

Ja, wenn ein Konflikt besteht, protokollieren wir das Ergebnis im Aktivitätsprotokoll des Leads.

>[!MORELIKETHIS]
>
>* [default [!DNL Veeva] field-mapping](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Meldungen zu Aufrufen und Aufrufen synchronisieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
