---
unique-page-id: 45417125
description: Sales Insight für nicht native Salesforce-Integrationen - Marketo Docs - Produktdokumentation
title: Sales Insight für nicht native Salesforce-Integrationen
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

# Sales Insight für nicht native Salesforce-Integrationen {#sales-insight-for-non-native-salesforce-integrations}

Wenn Ihr Adobe Marketo Engage-Konto über eine benutzerdefinierte oder nicht native Integration mit Salesforce verbunden ist, konfigurieren Sie in diesem Artikel Sales Insight.

>[!PREREQUISITES]
>
>* Die Funktion &quot;MSI Non-Native&quot;für Ihre Marketo-Instanz aktiviert, bevor Sie mit der Einrichtung von MSI beginnen. Wenn dies nicht der Fall ist und Sie die Funktion bereits erworben haben, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Wenn Sie diese Funktion noch nicht erworben haben, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer).
>* Ein Salesforce-Konto mit [eingerichtetem MSI-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* Marketo REST API [ wurde erfolgreich eingerichtet ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Die offen gelegten CRUD-APIs bilden die Grundlage für die Durchführung der nicht nativen Synchronisierung.
>* Lesen Sie [diesen Blogpost](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} , um ein Verständnis des Objekts und der Beziehungen zu erhalten.
>* Richten Sie Salesforce-Objekte so ein, dass die global eindeutige Kennung mit 18 Zeichen nicht von der Groß-/Kleinschreibung abhängig ist, sondern die globale eindeutige Kennung mit 15 Zeichen, bei der die Groß-/Kleinschreibung beachtet wird.

>[!NOTE]
>
>Die REST-API-Konfiguration im Marketo MSI Admin Panel kann nicht für die nicht native Synchronisierung verwendet werden.

## Für eine erfolgreiche nicht native Synchronisierung für MSI ist Folgendes erforderlich: {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisieren Sie den Salesforce Sales User mit Marketo.

   Salesforce Sales User ist ein externer Benutzer, der die Leads/Kontakte in Salesforce besitzt. Für den Salesforce Sales User muss eine Marketo Sales Person bereitgestellt werden. Das Feld *externalSalesPersonId* ist für die Aktualisierung der Verkaufsperson erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Sales Person Field</strong></td> 
      <td><strong>Salesforce Sales User Field</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei Salesforce Sales User wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td><p>Identifiziert den Marketo-Kundendatensatz für ein externes Salesforce Sales User-Objekt.</p><p>Es ist vorgeschrieben, dass die Vertriebsperson zuerst synchronisiert wird, bevor die anderen Objekte synchronisiert werden, damit die richtigen Beziehungen erstellt werden.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Vertriebsmitarbeiter: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * API-Dokumentation zum Synchronisieren der Vertriebsmitarbeiter: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisieren Sie die Salesforce-Konten mit Marketo.

   Ein Marketo-Unternehmen muss für das Salesforce-Konto aktualisiert werden. Die Felder _externalCompanyId_ und _externalSalesPersonId_ sind für die Aktualisierung des Unternehmens erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Firmenfeld</strong></td> 
      <td><strong>Salesforce-Kontofeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz für ein externes Salesforce-Kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei Salesforce Sales User wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz für ein externes Salesforce Sales User-Objekt, das der Kontoinhaber ist.<br><br>Wird auch innerhalb von Marketo verwendet, um das Unternehmen mit der Vertriebsperson zu verknüpfen, der der Firmendatensatz gehört. Es ist erforderlich, dass die Vertriebsperson zuerst synchronisiert wird, bevor dieses Feld festgelegt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Unternehmen: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * API-Dokumentation für die Synchronisierung von Unternehmen: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Synchronisieren Sie die Salesforce-Leads/Kontakte mit Marketo.

   Sie müssen einen Marketo Lead für Salesforce Lead/Kontakt aktualisieren. Die Felder _externalPersonId_, _externalSalesPersonId_ und _externalCompanyId_ sind für die Aktualisierung des Leads erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Lead-Feld</strong></td> 
      <td><strong>Salesforce Lead/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Bei Salesforce Lead/Contact wird die Groß-/Kleinschreibung nicht berücksichtigt - globale eindeutige Kennung</td> 
      <td>Identifiziert den Marketo Lead-Datensatz für ein externes Salesforce Lead-/Kontaktobjekt.<br><br>Dies ist ein neues Feld, das für MSI Non-Native eingeführt wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei Salesforce Sales User wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe Salesforce Sales User-Objekt, dem dieser Lead/Kontakt gehört.<br><br>Bezieht den Lead auch mit der Vertriebsperson in Marketo zusammen. Es ist erforderlich, dass die Vertriebsperson zuerst richtig synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem der Lead/Kontakt gehört.<br><br>Bezieht den Lead-Datensatz auch auf ein Unternehmen in Marketo. Es wird angewiesen, zunächst das Salesforce-Konto korrekt zu synchronisieren.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Leads: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)
   * API-Dokumentation zum Synchronisieren von Leads: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Salesforce-Chancen mit Marketo synchronisieren.

   Sie müssen eine Marketo-Chance für die Salesforce-Chancen unterstützen. Die Felder _externalOpportunityId_, _externalCompanyId_ und _externalSalesPersonId_ werden für die Aktualisierung der Chancen benötigt.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity Object Field</strong></td> 
      <td><strong>Salesforce Opportunity Object Field</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Bei Salesforce Lead/Contact wird die Groß-/Kleinschreibung nicht berücksichtigt - globale eindeutige Kennung</td> 
      <td>Identifiziert den Marketo Opportunity-Datensatz für ein externes Salesforce Opportunity-Objekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei Salesforce-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe Salesforce-Kontoobjekt, zu dem diese Gelegenheit gehört. <br><br>Es ist obligatorisch, dass das Salesforce-Konto zuerst richtig synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei Salesforce Sales User wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe Salesforce Sales User-Objekt, dem diese Gelegenheit gehört. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation für Synchronisierungsmöglichkeiten: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Salesforce-Kontaktrollen mit Marketo synchronisieren

   Salesforce-Kontaktrollen für eine Salesforce-Gelegenheit können dann über die Marketo-Opportunity-Rolle synchronisiert werden. Der Datensatz &quot;Opportunity Role&quot;erfordert die Felder _externalOpportunityId_, _role_ und _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity role Field</strong></td> 
      <td><strong>Salesforce-Kontaktrollenfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Bei Salesforce Opportunity wird die globale eindeutige Kennung nicht von der Groß-/Kleinschreibung unterschieden</td> 
      <td>Identifiziert die Marketo Opportunity-Rolle für ein externes Salesforce Opportunity-Objekt.<br><br>Es wird angewiesen, die Salesforce-Chancen zuerst richtig zu synchronisieren.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Nicht zutreffend: Dies wäre eine Marketo Lead-ID.</td> 
      <td>Dies wäre die Marketo-Lead-ID des synchronisierten Salesforce-Kontakts.<br><br>Nachdem der Kontakt in Marketo synchronisiert wurde, können Sie die global eindeutige Kennung Salesforce Contact ("Kontakt") als externalPersonId ("externalPersonId") und die Marketo Lead mithilfe der Marketo REST API abfragen.</td> 
     </tr> 
     <tr> 
      <td>Rolle</td> 
      <td>Das Rollenfeld für den Salesforce-Kontakt</td> 
      <td>Beschreibt die Rolle des Kontakts für diese Gelegenheit.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation für Synchronisierungsmöglichkeiten: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisieren Sie die letzten interessanten Moment-/MSI-Scoring-Felder mit SFDC.

   Sobald Ihre Salesforce-Objekte korrekt mit Marketo synchronisiert sind, können Sie die MSI-Funktionen nutzen. Die MSI-Felder Letzter interessanter Moment/Scoring werden in der REST-API für Leads angezeigt. Diese Felder werden durch MSI berechnet und sind schreibgeschützt.

   Die Felder &quot;Letzter interessanter Moment/Scoring&quot;eines Marketo-Leads müssen regelmäßig mit Salesforce über den REST-API-Lead-Endpunkt synchronisiert werden. Abfragen dieses Endpunkts für einen Marketo-Lead mit _externalPersonId_ als filterType und Übergabe der Salesforce-Lead-GUID als filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Sie können dann die Werte dieser Felder verwenden, um eine Synchronisation mit Ihrem Salesforce Lead-/Kontaktobjekt durchzuführen.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Lead-Feld</strong></td> 
      <td><strong>Salesforce Lead/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentType</td> 
      <td>Titel: Last Interest Moment Type<br>Name: Last_Interest_Moment_Type__c</td> 
      <td>Art des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDate</td> 
      <td><p>Titel: Letztes interessantes Datum</p><p>Name: Last_Interest_Moment_Date_c</p></td> 
      <td>Datum des letzten interessanten Augenblicks für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDesc</td> 
      <td><p>Titel: Letzter interessanter Moment - Beschreibung</p><p>Name: Last_Interest_Moment_Desc__c</p></td> 
      <td>Beschreibung des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentSource</td> 
      <td><p>Titel: Letzter interessanter Moment Source</p><p>Name: Last_Interest_Moment_Source__c</p></td> 
      <td>Source des letzten interessanten Augenblicks für die Führung</td> 
     </tr> 
     <tr> 
      <td>Priorität</td> 
      <td><p>Titel: Interaktion</p><p>Name: Priority__c</p></td> 
      <td>Priorität des Projektes</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Titel: Relativer Dringlichkeitswert</p><p>Name: Urgency_Value_c</p></td> 
      <td>Relativer Dringlichkeitsgrad des federführenden Unternehmens</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Titel: Relativer Scoring-Wert</p><p>Name: Relative_Score_Value_c</p></td> 
      <td>Relative Bewertung des Leads</td> 
     </tr> 
    </tbody> 
   </table>

   Dokumentation für die Lead-REST-API: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   Die ordnungsgemäße Verwendung der externen Felder ist für eine erfolgreiche, nicht native Synchronisierung von entscheidender Bedeutung. Wenn Sie in einigen Ansichten keine Daten sehen, wurde ein bestimmtes Feld wahrscheinlich nicht korrekt synchronisiert. Wenn beispielsweise die Aktivitäten und interessanten Momente eines Leads beim Betrachten des MSI-Widgets unter seinem Konto nicht angezeigt werden, ist es wahrscheinlich, dass entweder das Unternehmen des Leads oder das Konto nicht korrekt synchronisiert wurden. Wenn Sie eine GET-Anfrage für diesen Lead ausführen und die externen Felder angeben, können Sie überprüfen, ob der Lead richtig synchronisiert wurde. Darüber hinaus muss die E-Mail für die externe Vertriebsperson in Marketo mit der E-Mail-Adresse für diesen Benutzer in Salesforce übereinstimmen. Daten werden möglicherweise nicht auf der Registerkarte Marketo in Salesforce angezeigt, wenn die E-Mails nicht übereinstimmen.
