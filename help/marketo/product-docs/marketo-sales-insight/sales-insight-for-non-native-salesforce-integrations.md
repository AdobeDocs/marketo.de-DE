---
unique-page-id: 45417125
description: Sales Insight für nicht-native Salesforce-Integrationen - Marketing-Dokumente - Produktdokumentation
title: Sales Insight für nicht native Salesforce-Integrationen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Sales Insight für nicht native Salesforce-Integrationen {#sales-insight-for-non-native-salesforce-integrations}

Wenn Ihr Marketo-Konto über eine benutzerdefinierte oder nicht native Integration mit Salesforce verbunden ist, konfigurieren Sie mithilfe dieses Dokuments Sales Insight.

>[!PREREQUISITES]
>
>* Wenden Sie sich an Ihren Customer Success Manager, um die Funktion &quot;MSI Non-Native&quot;für Ihre Marketing-Instanz zu aktivieren.
>* Ein Salesforce-Konto mit MSI-Paket eingerichtet.
>* Marketo REST API [erfolgreich eingerichtet](http://developers.marketo.com/rest-api/). Die offen gelegten CRUD-APIs bilden die Grundlage für die Durchführung der nicht nativen Synchronisierung.
>* Lesen Sie [diesen Blog-Beitrag](http://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/), um ein Verständnis des Objekts und der Beziehungen zu erhalten.
>* Richten Sie Salesforce-Objekte so ein, dass der globale eindeutige Bezeichner mit 18 Zeichen und nicht der globale eindeutige Bezeichner mit 15 Zeichen ohne Unterscheidung zwischen Groß- und Kleinschreibung angezeigt wird.

>



>[!NOTE]
>
>Die REST-API-Konfiguration im Marketing MSI-Administrationsbedienfeld kann nicht für die native Synchronisierung verwendet werden.

## Für eine erfolgreiche, nicht native Synchronisierung für MSI ist Folgendes erforderlich: {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisieren Sie den Salesforce Sales User mit Marketo.

   Der Salesforce Sales User ist ein externer Benutzer, der Eigentümer der Leads/Kontakte in Salesforce ist. Eine Marketing-Vertriebsperson muss für den Salesforce-Vertriebsbenutzer aktualisiert werden. Das Feld *externalSalesPersonId* wird für die Aktualisierung der Vertriebsperson angefordert.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Feld "markto Sales Person"</strong></td> 
   <td><strong>Salesforce Sales User Field</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User unterscheidet nicht zwischen Groß- und Kleinschreibung bei der globalen eindeutigen Kennung</td> 
   <td><p>Identifiziert den Eintrag "Marketing-Verkaufsperson"in einem externen Salesforce Sales User-Objekt.</p><p>Es ist obligatorisch, dass die Vertriebsperson zuerst synchronisiert wird, bevor die anderen Objekte synchronisiert werden, damit die richtigen Beziehungen erstellt werden.</p></td> 
  </tr> 
 </tbody> 
</table>

API-Dokumentation für Vertriebsmitarbeiter: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](http://developers.marketo.com/rest-api/lead-database/sales-persons/)\
API-Dokumentation für die Synchronisierung der Vertriebsperson: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. Synchronisieren Sie die Salesforce-Konten mit Marketo.

   Für das Salesforce-Konto muss eine Marketo-Firma aktualisiert werden. Die Felder *externalCompanyId* und *externalSalesPersonId* werden für die Aktualisierung der Firma angefordert.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Feld "Firma"</strong></td> 
   <td><strong>Salesforce-Kontofeld</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
   <td>Identifiziert einen Marketo-Firmen-Datensatz zu einem externen Salesforce-Kontoobjekt.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User unterscheidet nicht zwischen Groß- und Kleinschreibung bei der globalen eindeutigen Kennung</td> 
   <td>Identifiziert einen Marketo-Firma-Datensatz für ein externes Salesforce Sales User-Objekt, das der Kontoinhaber ist.<br><br>Wird auch innerhalb von Marketo verwendet, um die Firma mit der Vertriebsperson zu verknüpfen, der der Datensatz zur Firma gehört. Es ist erforderlich, dass die Vertriebsperson zuerst synchronisiert wird, bevor dieses Feld festgelegt wird.</td> 
  </tr> 
 </tbody> 
</table>

API-Dokumentation für Firmen: [https://developers.marketo.com/rest-api/lead-database/companies/](http://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Synchronisieren Sie die Salesforce Leads/Kontakte mit Marketo.

   Sie müssen einen Marketo Lead für den Salesforce Lead/Kontakt aufstellen. Die Felder *externalPersonId*, *externalSalesPersonId* und *externalCompanyId* sind für die Aktualisierung des Interessenten obligatorisch.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Interessentenfeld von Marketing</strong></td> 
   <td><strong>Salesforce-Interessent-/Kontaktfeld</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Bei Salesforce Lead/Kontaktperson wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
   <td>Identifiziert den Marketo-Interessentendatensatz zu einem externen Salesforce-Lead-/Kontaktobjekt.<br><br>Dies ist ein neues Feld, das für MSI Non-Native eingeführt wird.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User unterscheidet nicht zwischen Groß- und Kleinschreibung bei der globalen eindeutigen Kennung</td> 
   <td>Identifiziert das externe Salesforce Sales User-Objekt, dem dieser Interessent/Kontakt gehört.<br><br>Bezieht sich auch auf den Lead mit der Verkaufsperson in Marketo. Es ist obligatorisch, dass die Vertriebsperson zuerst richtig synchronisiert wird.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
   <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem der Interessent/Kontakt gehört.<br><br>Bezieht sich auch den Interessentenrekord auf eine Firma in Marketo. Es ist obligatorisch, zuerst das Salesforce-Konto korrekt zu synchronisieren.</td> 
  </tr> 
 </tbody> 
</table>

API-Dokumentation für Interessenten: [`https://developers.marketo.com/rest-api/lead-database/leads/`](http://developers.marketo.com/rest-api/lead-database/leads/)\
API-Dokumentation für die Synchronisierung von Interessenten:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Synchronisieren Sie Salesforce-Chancen mit Marketo.

   Für die Salesforce-Gelegenheit müssen Sie eine Marketing-Chance aktualisieren. Die Felder *externalOpportunityId*, *externalCompanyId* und *externalSalesPersonId* sind für die Aktualisierung der Gelegenheit obligatorisch.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Objektfeld "Marketing-Gelegenheit"</strong></td> 
   <td><strong>Salesforce-Objektfeld</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Bei Salesforce Lead/Kontaktperson wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
   <td>Identifiziert den Marketo-Opportunity-Datensatz für ein externes Salesforce-Opportunity-Objekt.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
   <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem diese Gelegenheit gehört. <br><br>Es ist obligatorisch, zuerst das Salesforce-Konto korrekt zu synchronisieren.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User unterscheidet nicht zwischen Groß- und Kleinschreibung bei der globalen eindeutigen Kennung</td> 
   <td>Identifiziert das externe Salesforce Sales User-Objekt, dem diese Gelegenheit gehört. </td> 
  </tr> 
 </tbody> 
</table>

API-Dokumentation für Chancen: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synchronisieren Sie Salesforce-Kontaktrollen mit Marketo.

   Salesforce-Kontaktrollen für eine Salesforce-Chance können dann über die Marketing-Opportunity-Rolle synchronisiert werden. Der Bericht &quot;Opportunity Role&quot;fordert die Felder *externalOpportunityId*, *role* und *leadId* auf.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Feld für die Rolle von Marketo-Chancen</strong></td> 
   <td><strong>Kontaktfeld für Salesforce</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Bei Salesforce Opportunity wird die Groß-/Kleinschreibung nicht beachtet.</td> 
   <td>Identifiziert die Rolle "Marketo-Chancen"mit einem externen Salesforce-Opportunity-Objekt.<br><br>Es wird vorgeschrieben, dass die Salesforce-Gelegenheit zuerst richtig synchronisiert werden muss.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>Nicht zutreffend: Dies wäre eine Marketing Lead-ID.</td> 
   <td>Dies wäre die Marketing Lead-ID des synchronisierten Salesforce-Kontakts.<br><br>Nachdem der Kontakt in Marketo synchronisiert wurde, können Sie den global eindeutigen Bezeichner Salesforce Contact ohne Unterscheidung der Groß-/Kleinschreibung als externalPersonId und Abfrage für den MarketingTo Lead mit der MarketingTo REST API verwenden.</td> 
  </tr> 
  <tr> 
   <td>role</td> 
   <td>Das Feld Rolle für den Salesforce-Kontakt</td> 
   <td>Beschreibt die Rolle des Kontakts für diese Gelegenheit.</td> 
  </tr> 
 </tbody> 
</table>

API-Dokumentation für Chancen: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synchronisieren Sie die Felder &quot;Letzter interessanter Moment/MSI-Scoring&quot;mit dem SFDC.

   Sobald Ihre Salesforce-Objekte korrekt mit Marketo synchronisiert wurden, können Sie die MSI-Funktionen nutzen. Die Felder &quot;Letzter interessanter Moment/Bewertung&quot;für MSI werden in der REST-API für Interessenten angezeigt. Diese Felder werden durch MSI berechnet und sind schreibgeschützt.

   Die Felder &quot;Letzter interessanter Moment/Bewertung&quot;eines Marketo-Interessenten müssen regelmäßig mit Salesforce unter Verwendung des REST API-Interessentenendpunkts synchronisiert werden. Abfrage dieses Endpunkts für einen Marketo-Lead mit der *externalPersonId* als filterType und Übergabe der Salesforce-Lead-GUID als filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Mithilfe der Werte dieser Felder können Sie dann mit Ihrem Salesforce-Lead-/Kontaktobjekt synchronisieren.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Interessentenfeld von Marketing</strong></td> 
   <td><strong>Salesforce-Interessent-/Kontaktfeld</strong></td> 
   <td><strong>Beschreibung</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInteressentMomentType</td> 
   <td>Beschriftung: Letzter interessanter Moment Typ<br>Name: last_interessante_moment_type_c</td> 
   <td>Art des letzten interessanten Moments für den Interessenten</td> 
  </tr> 
  <tr> 
   <td>msiLastInteressentMomentDate</td> 
   <td><p>Beschriftung: Datum des letzten interessanten Moments</p><p>Name: last_interessante_moment_date__c</p></td> 
   <td>Datum des letzten interessanten Moments für den Interessenten des Interessenten</td> 
  </tr> 
  <tr> 
   <td>msiLastInteressentMomentDesc</td> 
   <td><p>Beschriftung: Beschreibung des letzten interessanten Moments</p><p>Name: last_interessante_moment_desc__c</p></td> 
   <td>Beschreibung des letzten interessanten Moments für den Interessenten</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestedMomentSource</td> 
   <td><p>Beschriftung: Letzter interessanter Moment Quelle</p><p>Name: Last_Interest_Moment_Source_c</p></td> 
   <td>Quelle des letzten interessanten Moments für den Interessenten</td> 
  </tr> 
  <tr> 
   <td>Priorität</td> 
   <td><p>Beschriftung: Interaktion</p><p>Name: Priority__c</p></td> 
   <td>Priorität des Interessenten</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>Beschriftung: Relativer Dringlichkeitswert</p><p>Name: Urgency_Value__c</p></td> 
   <td>Relative Dringlichkeit des Interessenten</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Beschriftung: Relativer Bewertungswert</p><p>Name: Relative_Score_Value_c</p></td> 
   <td>Relative Bewertung des Interessenten</td> 
  </tr> 
 </tbody> 
</table>

Dokumentation für die Interessenten-REST-API:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

Die ordnungsgemäße Verwendung der externen Felder ist der Schlüssel für eine erfolgreiche, nicht native Synchronisierung. Wenn in einigen Ansichten keine Daten angezeigt werden, wurde ein bestimmtes Feld wahrscheinlich nicht korrekt synchronisiert. Wenn beispielsweise die Aktivitäten und interessanten Momente eines Interessenten beim Betrachten des MSI-Widgets unter seinem Konto nicht angezeigt werden, ist es wahrscheinlich, dass entweder die Firma des Interessenten oder das Konto nicht richtig synchronisiert wurde. Wenn Sie eine GET für diesen Interessenten durchführen und dabei die externen Felder angeben, können Sie überprüfen, ob der Interessent richtig synchronisiert wurde. Darüber hinaus muss die E-Mail für den externen Vertriebsmitarbeiter in Marketo mit der E-Mail für diesen Benutzer in Salesforce übereinstimmen. Daten werden in Salesforce auf der Registerkarte &quot;Markieren&quot;möglicherweise nicht angezeigt, wenn die E-Mails nicht übereinstimmen.

