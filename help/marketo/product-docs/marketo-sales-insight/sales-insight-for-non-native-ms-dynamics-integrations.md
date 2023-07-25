---
description: Sales Insight für nicht native MS Dynamics-Integrationen - Marketo Docs - Produktdokumentation
title: Sales Insight für nicht native MS Dynamics-Integrationen
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# Sales Insight für nicht native MS Dynamics-Integrationen {#sales-insight-for-non-native-ms-dynamics-integrations}

Wenn Ihr Adobe Marketo Engage-Konto über eine benutzerdefinierte oder nicht native Integration mit MS Dynamics verbunden ist, konfigurieren Sie in diesem Artikel Sales Insight.

>[!PREREQUISITES]
>
>* Die Funktion &quot;MSI Non-Native&quot;für Ihre Marketo-Instanz aktiviert, bevor Sie mit der Einrichtung von MSI beginnen. Wenn dies nicht der Fall ist und Sie die Funktion bereits erworben haben, wenden Sie sich an [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Wenn Sie diese Funktion noch nicht erworben haben, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer).
>* Download [MSI-Paket für benutzerdefinierte Synchronisierung](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Ein MS Dynamics-Abonnement mit MSI-Einrichtung (wir unterstützen nur [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} ).
>* Marketo REST API [erfolgreich einrichten](https://developers.marketo.com/rest-api/){target="_blank"}. Die offen gelegten CRUD-APIs bilden die Grundlage für die Durchführung der nicht nativen Synchronisierung.
>* Lesen [Dieser Blogpost](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} um ein Verständnis des Objekts und der Beziehungen zu erhalten.

## Für eine erfolgreiche nicht native Synchronisierung für MSI ist Folgendes erforderlich: {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisieren Sie den MS Dynamics Sales User mit Marketo.

   Der MS Dynamics Sales User ist ein externer Benutzer, der die Leads/Kontakte in MS Dynamics besitzt. Für den MS Dynamics Sales User muss eine Marketo Sales Person bereitgestellt werden. Das Feld externalSalesPersonId ist für die Aktualisierung der Vertriebsperson erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Sales Person Field</strong></td> 
      <td><strong>MS Dynamics-Benutzerfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei MS Dynamics-Benutzern wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td><p>Identifiziert den Marketo Sales Person-Datensatz für ein externes MS Dynamics User-Objekt.</p><p>Es ist vorgeschrieben, dass die Vertriebsperson zuerst synchronisiert wird, bevor die anderen Objekte synchronisiert werden, damit die richtigen Beziehungen erstellt werden.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Vertriebsmitarbeiter: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * API-Dokumentation für die Synchronisierung der Vertriebsperson: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisieren Sie die MS Dynamics-Konten mit Marketo.

   Ein Marketo-Unternehmen muss für das MS Dynamics-Konto aktualisiert werden. Die _externalCompanyId_ und _externalSalesPersonId_ -Felder sind für die Aktualisierung des Unternehmens erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Firmenfeld</strong></td> 
      <td><strong>MS Dynamics-Kontofeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei MS Dynamics-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz für ein externes MS Dynamics-Kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei MS Dynamics Sales-Benutzern wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz für ein externes MS Dynamics Sales User-Objekt, das der Kontoinhaber ist.<br><br>Wird auch innerhalb von Marketo verwendet, um das Unternehmen mit der Vertriebsperson zu verknüpfen, der der Datensatz "Unternehmen"gehört. Es ist erforderlich, dass die Vertriebsperson zuerst synchronisiert wird, bevor dieses Feld festgelegt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Unternehmen: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * API-Dokumentation für die Synchronisierung von Unternehmen: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. Synchronisieren Sie die MS Dynamics-Leads/Kontakte mit Marketo.

   Sie müssen einen Marketo Lead für den MS Dynamics Lead/Kontakt aktualisieren. Die _externalPersonId_, _externalSalesPersonId_ und _externalCompanyId_ -Felder sind für die Aktualisierung des Leads erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Lead-Feld</strong></td> 
      <td><strong>MS Dynamics Lead-/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Bei MS Dynamics Lead/Contact wird die Groß-/Kleinschreibung nicht berücksichtigt, globale eindeutige Kennung</td> 
      <td>Identifiziert den Marketo-Lead-Datensatz für ein externes MS Dynamics Lead-/Contact-Objekt.<br><br>Dies ist ein neues Feld, das für MSI Non-Native eingeführt wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei MS Dynamics Sales-Benutzern wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
      <td>Identifiziert das externe MS Dynamics Sales User-Objekt, dem dieser Lead/Kontakt gehört.<br><br>Bezieht auch den Lead mit der Vertriebsmitarbeiterin in Marketo zusammen. Es ist erforderlich, dass die Vertriebsperson zuerst richtig synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei MS Dynamics-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe MS Dynamics-Kontoobjekt, zu dem der Lead/Kontakt gehört.<br><br>Bezieht den Lead-Datensatz auch auf ein Unternehmen in Marketo. Es ist erforderlich, dass das MS Dynamics-Konto zuerst richtig synchronisiert wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Leads: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target="_blank"}
   * API-Dokumentation für die Synchronisierung von Leads: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target="_blank"}

1. Synchronisieren von MS Dynamics-Chancen mit Marketo.

   Sie müssen eine Marketo-Chance für die MS Dynamics-Chancen unterstützen. Die _externalOpportunityId_, _externalCompanyId_ und _externalSalesPersonId_ -Felder sind für die Aktualisierung der Option erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity Object Field</strong></td> 
      <td><strong>MS Dynamics Opportunity Object Field</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Bei MS Dynamics Lead/Contact wird die Groß-/Kleinschreibung nicht berücksichtigt, globale eindeutige Kennung</td> 
      <td>Identifiziert den Marketo Opportunity-Datensatz für ein externes MS Dynamics Opportunity-Objekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Bei MS Dynamics-Konten wird nicht zwischen Groß- und Kleinschreibung unterschieden - globale eindeutige Kennung</td> 
      <td>Identifiziert das externe MS Dynamics-Kontoobjekt, zu dem diese Gelegenheit gehört. <br><br>Es ist erforderlich, dass das MS Dynamics-Konto zuerst richtig synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Bei MS Dynamics Sales-Benutzern wird nicht zwischen Groß- und Kleinschreibung unterschieden.</td> 
      <td>Identifiziert das externe MS Dynamics Sales User-Objekt, dem diese Gelegenheit gehört. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * API-Dokumentation für Synchronisierungsmöglichkeiten: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisieren von MS Dynamics-Kontaktrollen mit Marketo.

   MS Dynamics-Kontaktrollen für eine MS Dynamics-Chance können dann über die Marketo Opportunity-Rolle synchronisiert werden. Der Datensatz &quot;Opportunity Role&quot;weist die _externalOpportunityId_, _Rolle_ und _leadId_ -Felder.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity role Field</strong></td> 
      <td><strong>MS Dynamics-Kontaktrollenfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Bei MS Dynamics Opportunity wird die Groß-/Kleinschreibung nicht berücksichtigt, global eindeutige Kennung</td> 
      <td>Identifiziert die Marketo Opportunity-Rolle für ein externes MS Dynamics Opportunity-Objekt.<br><br>Es wird angewiesen, die MS Dynamics-Chancen zuerst richtig zu synchronisieren.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Nicht zutreffend: Dies wäre eine Marketo Lead-ID.</td> 
      <td>Dies wäre die Marketo-Lead-ID des synchronisierten MS Dynamics-Kontakts.<br><br>Nachdem der Kontakt in Marketo synchronisiert wurde, können Sie die global eindeutige Kennung MS Dynamics Contact verwenden, die nicht von der Schreibweise abhängig ist, als externalPersonId und die Abfrage für Marketo Lead mithilfe der Marketo REST API.</td> 
     </tr> 
     <tr> 
      <td>Rolle</td> 
      <td>Das Rollenfeld für den MS Dynamics-Kontakt</td> 
      <td>Beschreibt die Rolle des Kontakts für diese Gelegenheit.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * API-Dokumentation für Synchronisierungsmöglichkeiten: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisieren Sie die letzten interessanten Moment-/MSI-Scoring-Felder mit MS Dynamics.

   Sobald Ihre MS Dynamics-Objekte korrekt mit Marketo synchronisiert sind, können Sie die MSI-Funktionen nutzen. Die MSI-Felder Letzter interessanter Moment/Scoring werden in der REST-API für Leads angezeigt. Diese Felder werden durch MSI berechnet und sind schreibgeschützt.

   Die letzten interessanten Moment-/Scoring-Felder eines Marketo Leads müssen regelmäßig mit MS Dynamics über den REST API Lead-Endpunkt synchronisiert werden. Abfragen dieses Endpunkts für einen Marketo-Lead mithilfe der _externalPersonId_ als filterType und Übergabe der MS Dynamics Lead GUID als filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Sie können dann die Werte dieser Felder verwenden, um eine Synchronisierung mit Ihrem MS Dynamics Lead-/Kontaktobjekt durchzuführen.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Lead-Feld</strong></td> 
      <td><strong>MS Dynamics Lead-/Kontaktfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentType</td> 
      <td>Titel: Letzter interessanter Moment-Typ<br>Name: last_interessante_moment_type_c</td> 
      <td>Art des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDate</td> 
      <td><p>Titel: Letztes interessantes Datum</p><p>Name: Last_Interest_Moment_Date_c</p></td> 
      <td>Datum des letzten interessanten Augenblicks für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDesc</td> 
      <td><p>Titel: Beschreibung des letzten interessanten Moments</p><p>Name: last_interessante_moment_desc__c</p></td> 
      <td>Beschreibung des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentSource</td> 
      <td><p>Titel: Letzte interessante Moment-Quelle</p><p>Name: Last_Interest_Moment_Source_c</p></td> 
      <td>Quelle des letzten interessanten Moments für den Lead</td> 
     </tr> 
     <tr> 
      <td>Priorität</td> 
      <td><p>Titel: Interaktion</p><p>Name: Priority_c</p></td> 
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

   * Dokumentation zur Lead-REST-API: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   Die ordnungsgemäße Verwendung der externen Felder ist für eine erfolgreiche nicht native Synchronisierung von entscheidender Bedeutung. Wenn Sie in einigen Ansichten keine Daten sehen, wurde ein bestimmtes Feld wahrscheinlich nicht korrekt synchronisiert. Wenn beispielsweise die Aktivitäten und interessanten Momente eines Leads beim Betrachten des MSI-Widgets unter seinem Konto nicht angezeigt werden, ist es wahrscheinlich, dass entweder das Unternehmen des Leads oder das Konto nicht korrekt synchronisiert wurden. Wenn Sie eine GET-Anfrage für diesen Lead ausführen und die externen Felder angeben, können Sie überprüfen, ob der Lead richtig synchronisiert wurde. Darüber hinaus muss die E-Mail für die externe Vertriebsperson in Marketo mit der E-Mail-Adresse für diesen Benutzer in MS Dynamics übereinstimmen. Daten werden auf der Registerkarte Marketo in MS Dynamics möglicherweise nicht angezeigt, wenn die E-Mails nicht übereinstimmen.
