---
unique-page-id: 45417125
description: Sales Insight für nicht-native Salesforce-Integrationen - Marketo-Dokumente - Produktdokumentation
title: Sales Insight für nicht-native Salesforce-Integrationen
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

# Sales Insight für nicht-native Salesforce-Integrationen {#sales-insight-for-non-native-salesforce-integrations}

Wenn Ihr Adobe Marketo Engage-Konto über eine benutzerdefinierte oder nicht native Integration mit Salesforce verbunden ist, konfigurieren Sie in diesem Artikel Sales Insight.

>[!PREREQUISITES]
>
>* Die Funktion „MSI Non-Native“ wurde für Ihre Marketo-Instanz aktiviert, bevor Sie mit der Einrichtung von MSI beginnen. Wenn dies nicht der Fall ist und Sie die Funktion bereits erworben haben, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Wenn Sie diese Funktion noch nicht erworben haben, wenden Sie sich an das Adobe Account Team (Ihren Account Manager).
>* Ein Salesforce-Konto mit [MSI-Paket eingerichtet](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* Marketo REST-API [erfolgreich eingerichtet](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Die offen gelegten CRUD-APIs sind die Grundlage für die Durchführung der nicht nativen Synchronisierung.
>* Lesen Sie [diesen Blogpost](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"}, um ein Verständnis des Objekts und der Beziehungen zu erhalten.
>* Richten Sie Salesforce-Objekte so ein, dass die globale eindeutige Kennung, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird, anstelle der globalen eindeutigen Kennung, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird, bei 15 Zeichen angezeigt wird.

>[!NOTE]
>
>Die REST-API-Konfiguration im Marketo MSI Admin Panel kann nicht für die nicht native Synchronisierung verwendet werden.

## Für eine erfolgreiche nicht-native Synchronisation für MSI ist Folgendes erforderlich {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisieren Sie den Salesforce Sales User mit Marketo.

   Der Salesforce-Verkaufsbenutzer ist ein externer Benutzer, dem die Leads/Kontakte in Salesforce gehören. Ein Marketo-Vertriebsmitarbeiter muss für den Salesforce-Vertriebsmitarbeiter upsertiert werden. Das Feld *externalSalesPersonId* ist für das Upsert der Verkaufsperson erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Feld für Vertriebsperson</strong></td> 
      <td><strong>Salesforce Sales User Field</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung beim Salesforce-Vertrieb</td> 
      <td><p>Identifiziert den Datensatz "Marketo Sales Person“ in einem externen Salesforce Sales User-Objekt.</p><p>Es wird vorgeschrieben, dass der Vertriebsmitarbeiter zuerst synchronisiert wird, bevor die anderen Objekte synchronisiert werden, damit die richtigen Beziehungen erstellt werden.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Vertriebsperson: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * API-Dokumentation zum Synchronisieren der Vertriebsperson: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisieren Sie die Salesforce-Konten mit Marketo.

   Eine Marketo-Firma muss für das Salesforce-Konto upsertiert werden. Die Felder _externalCompanyId_ und _externalSalesPersonId_ sind für das Upsert des Unternehmens erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Unternehmensfeld</strong></td> 
      <td><strong>Salesforce-Kontofeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für das Salesforce-Konto</td> 
      <td>Identifiziert einen Unternehmensdatensatz in Marketo in einem externen Salesforce-Kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung beim Salesforce-Vertrieb</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz in einem externen Salesforce-Verkaufsbenutzerobjekt, das Kontoinhaber ist.<br><br>Wird auch in Marketo verwendet, um die Firma mit dem Vertriebspersonal zu verknüpfen, dem der Firmendatensatz gehört. Es ist erforderlich, dass der Verkäufer zuerst synchronisiert wird, bevor dieses Feld festgelegt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Unternehmen: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * API-Dokumentation für das Synchronisieren von Unternehmen: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Synchronisieren Sie die Salesforce-Leads/-Kontakte mit Marketo.

   Sie müssen einen Marketo-Lead für den Salesforce-Lead/-Kontakt upsertieren. Die Felder _externalPersonId_, _externalSalesPersonId_ und _externalCompanyId_ sind für das Upsert des Leads erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead-Feld</strong></td> 
      <td><strong>Salesforce Lead/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei Salesforce Lead/Kontakt</td> 
      <td>Identifiziert den Marketo-Lead-Eintrag zu einem externen Salesforce-Lead/Kontaktobjekt.<br><br>Dies ist ein neues Feld, das für MSI Non-Native eingeführt wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung beim Salesforce-Vertrieb</td> 
      <td>Identifiziert das externe Salesforce Sales-Benutzerobjekt, dem dieser Lead/Kontakt gehört.<br><br>Bezieht den Lead auch mit dem Vertriebspersonal in Marketo. Es ist erforderlich, dass die Vertriebsperson zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für das Salesforce-Konto</td> 
      <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem der Lead/Kontakt gehört.<br><br>Bezieht den Lead-Datensatz auch auf eine Firma in Marketo. Es wird vorgeschrieben, dass das Salesforce-Konto zuerst korrekt synchronisiert wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Leads: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/leads)
   * API-Dokumentation zum Synchronisieren von Leads: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Synchronisieren Sie Salesforce-Opportunities mit Marketo.

   Sie müssen eine Marketo-Opportunity für die Salesforce-Opportunity upsertieren. Die Felder _externalOpportunityId_, _externalCompanyId_ und _externalSalesPersonId_ werden für das Upsert der Opportunity benötigt.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity-Objektfeld</strong></td> 
      <td><strong>Salesforce Opportunity-Objektfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei Salesforce Lead/Kontakt</td> 
      <td>Identifiziert den Marketo Opportunity-Datensatz für ein externes Salesforce Opportunity-Objekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für das Salesforce-Konto</td> 
      <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem diese Opportunity gehört. <br><br>Es ist erforderlich, dass das Salesforce-Konto zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung beim Salesforce-Vertrieb</td> 
      <td>Identifiziert das externe Salesforce Sales-Benutzerobjekt, dem diese Opportunity gehört. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation zum Synchronisieren von Opportunities: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisieren Sie Salesforce-Kontaktrollen mit Marketo.

   Kontaktrollen von Salesforce für eine Opportunity in Salesforce können dann über die Opportunity-Rolle von Marketo synchronisiert werden. Der Datensatz für die Opportunity-Rolle erfordert die Felder _externalOpportunityId_, _role_ und _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity-Rollenfeld</strong></td> 
      <td><strong>Salesforce-Kontaktrollenfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung bei Salesforce-Opportunity</td> 
      <td>Identifiziert die Opportunity-Rolle von Marketo in einem externen Opportunity-Objekt von Salesforce.<br><br>Es wird vorgeschrieben, dass die Salesforce-Opportunity zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Nicht zutreffend, dies wäre eine Marketo Lead-ID.</td> 
      <td>Dies ist die Marketo-Lead-ID des synchronisierten Salesforce-Kontakts.<br><br>Nachdem der Kontakt in Marketo synchronisiert wurde, können Sie die eindeutige Kennung "Salesforce Contact“ ohne Berücksichtigung der Groß-/Kleinschreibung als externalPersonId verwenden und mit der Marketo REST-API eine Abfrage für den Marketo-Lead durchführen.</td> 
     </tr> 
     <tr> 
      <td>Rolle</td> 
      <td>Das Rollenfeld für den Salesforce-Kontakt</td> 
      <td>Beschreibt die Rolle des Kontakts für diese Opportunity.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation zum Synchronisieren von Opportunities: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisieren Sie die Bewertungsfelder „Letzter interessanter Moment/MSI“ mit SFDC.

   Sobald Ihre Salesforce-Objekte korrekt mit Marketo synchronisiert wurden, können Sie die MSI-Funktionen nutzen. Die Felder für den letzten interessanten MSI-Moment/die letzte Bewertung werden in der REST-API für Leads angezeigt. Diese Felder werden von MSI berechnet und sind schreibgeschützt.

   Die Felder „Letzter interessanter Moment/letzte Bewertung“ eines Marketo-Leads müssen regelmäßig mithilfe des Lead-Endpunkts der REST-API mit Salesforce synchronisiert werden. Fragen Sie diesen Endpunkt für einen Marketo-Lead mit _externalPersonId_ als filterType ab und übergeben Sie die Salesforce-Lead-GUID als filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Sie können dann die Werte dieser Felder verwenden, um sie mit Ihrem Salesforce Lead/Kontaktobjekt zu synchronisieren.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead-Feld</strong></td> 
      <td><strong>Salesforce Lead/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Bezeichnung: Letzter interessanter Moment Typ<br>Name: Last_Interesting_Moment_Type__c</td> 
      <td>Typ des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Beschriftung: Datum des letzten interessanten Moments</p><p>Name: last_interesting_moment_date__c</p></td> 
      <td>Datum des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Titel: Beschreibung des letzten interessanten Moments</p><p>Name: last_interesting_moment_desc__c</p></td> 
      <td>Beschreibung des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Titel: Last Interesting Moment Source</p><p>Name: last_interesting_moment_Source__c</p></td> 
      <td>Source des letzten interessanten Augenblicks für den Lead</td> 
     </tr> 
     <tr> 
      <td>Priorität</td> 
      <td><p>Bezeichnung: Interaktion</p><p>Name: priority__c</p></td> 
      <td>Priorität des Leads</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Titel: relativer Dringlichkeitswert</p><p>Name: URIGITY_VALUE__c</p></td> 
      <td>Relative Dringlichkeit des Leads</td> 
     </tr> 
     <tr> 
      <td>relative Bewertung</td> 
      <td><p>Titel: Relativer Wert der Bewertung</p><p>Name: relative_score_value__c</p></td> 
      <td>Relative Bewertung des Leads</td> 
     </tr> 
    </tbody> 
   </table>

   Dokumentation für die Lead-REST-API: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   Die ordnungsgemäße Verwendung der externen Felder ist der Schlüssel für eine erfolgreiche nicht-native Synchronisation. Wenn in einigen Ansichten keine Daten angezeigt werden, ist es wahrscheinlich, dass ein bestimmtes Feld nicht korrekt synchronisiert wurde. Wenn beispielsweise die Aktivitäten und interessanten Momente eines Leads beim Anzeigen im MSI-Widget unter seinem Konto nicht angezeigt werden, ist es wahrscheinlich, dass entweder das Unternehmen des Leads oder das Konto nicht korrekt synchronisiert wurde. Wenn Sie eine GET-Anfrage für diesen Lead ausführen und dabei die externen Felder angeben, können Sie überprüfen, ob der Lead korrekt synchronisiert wurde. Darüber hinaus muss die E-Mail für den externen Vertriebspersonal in Marketo mit der E-Mail für diesen Benutzer in Salesforce übereinstimmen. Daten werden in Salesforce möglicherweise nicht auf der Registerkarte Marketo angezeigt, wenn die E-Mails nicht übereinstimmen.
