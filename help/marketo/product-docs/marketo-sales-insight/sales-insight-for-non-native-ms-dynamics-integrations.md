---
description: Sales Insight für nicht-native MS Dynamics-Integrationen - Marketo-Dokumente - Produktdokumentation
title: Sales Insight für nicht-native MS Dynamics-Integrationen
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Sales Insight für nicht-native MS Dynamics-Integrationen {#sales-insight-for-non-native-ms-dynamics-integrations}

Wenn Ihr Adobe Marketo Engage-Konto über eine benutzerdefinierte oder nicht native Integration mit MS Dynamics verbunden ist, konfigurieren Sie in diesem Artikel Sales Insight.

>[!PREREQUISITES]
>
>* Die Funktion „MSI Non-Native“ wurde für Ihre Marketo-Instanz aktiviert, bevor Sie mit der Einrichtung von MSI beginnen. Wenn dies nicht der Fall ist und Sie die Funktion bereits erworben haben, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Wenn Sie diese Funktion noch nicht erworben haben, wenden Sie sich an das Adobe Account Team (Ihren Account Manager).
>* Laden Sie [MSI-Paket für benutzerdefinierte Synchronisierung](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"} herunter.
>* Ein MS Dynamics-Abonnement mit MSI-Setup (derzeit wird [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} nur unterstützt).
>* Marketo REST-API [erfolgreich eingerichtet](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Die offen gelegten CRUD-APIs sind die Grundlage für die Durchführung der nicht nativen Synchronisierung.
>* Lesen Sie [diesen Blogpost](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"}, um ein Verständnis des Objekts und der Beziehungen zu erhalten.

## Für eine erfolgreiche nicht-native Synchronisation für MSI ist Folgendes erforderlich {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisieren Sie den MS Dynamics-Verkaufsbenutzer mit Marketo.

   Der MS Dynamics-Verkaufsbenutzer ist ein externer Benutzer, dem die Leads/Kontakte in MS Dynamics gehören. Ein Marketo-Vertriebsmitarbeiter muss für den MS Dynamics-Vertriebsbenutzer upsertiert werden. Das Feld externalSalesPersonId wird für das Upsert der Sales-Person benötigt.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Feld für Vertriebsperson</strong></td> 
      <td><strong>MS Dynamics-Benutzerfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung bei MS Dynamics</td> 
      <td><p>Identifiziert den Datensatz "Marketo Sales Person“ in einem externen MS Dynamics-Benutzerobjekt.</p><p>Es wird vorgeschrieben, dass der Vertriebsmitarbeiter zuerst synchronisiert wird, bevor die anderen Objekte synchronisiert werden, damit die richtigen Beziehungen erstellt werden.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [API-Dokumentation für Vertriebsmitarbeiter](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [API-Dokumentation zum Synchronisieren des Vertriebspersonals](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisieren Sie die MS Dynamics-Konten mit Marketo.

   Eine Marketo-Firma muss für das MS Dynamics-Konto upsertiert werden. Die Felder _externalCompanyId_ und _externalSalesPersonId_ sind für das Upsert des Unternehmens erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-Unternehmensfeld</strong></td> 
      <td><strong>MS Dynamics-Kontofeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für MS Dynamics-Konto</td> 
      <td>Identifiziert einen Marketo-Unternehmensdatensatz in einem externen MS Dynamics-Kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei MS Dynamics Sales</td> 
      <td>Identifiziert einen Marketo-Firmendatensatz in einem externen MS Dynamics-Verkaufsbenutzerobjekt, das Kontoinhaber ist.<br><br>Wird auch in Marketo verwendet, um die Firma mit dem Vertriebspersonal zu verknüpfen, dem der Firmendatensatz gehört. Es ist erforderlich, dass der Verkäufer zuerst synchronisiert wird, bevor dieses Feld festgelegt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Unternehmen: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * API-Dokumentation für das Synchronisieren von Unternehmen: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisieren Sie die MS Dynamics-Leads/-Kontakte mit Marketo.

   Sie müssen einen Marketo-Lead für den MS Dynamics-Lead/Kontakt upsertieren. Die Felder _externalPersonId_, _externalSalesPersonId_ und _externalCompanyId_ sind für das Upsert des Leads erforderlich.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead-Feld</strong></td> 
      <td><strong>MS Dynamics Lead/Kontakt-Feld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei MS Dynamics Lead/Kontakt</td> 
      <td>Identifiziert den Marketo-Lead-Datensatz für ein externes MS Dynamics-Lead-/Kontaktobjekt.<br><br>Dies ist ein neues Feld, das für MSI Non-Native eingeführt wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei MS Dynamics Sales</td> 
      <td>Identifiziert das externe MS Dynamics-Verkaufsbenutzerobjekt, dem dieser Lead/Kontakt gehört.<br><br>Bezieht den Lead auch mit dem Vertriebspersonal in Marketo. Es ist erforderlich, dass die Vertriebsperson zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für MS Dynamics-Konto</td> 
      <td>Identifiziert das externe MS Dynamics-Kontoobjekt, zu dem der Lead/Kontakt gehört.<br><br>Bezieht den Lead-Datensatz auch auf eine Firma in Marketo. Es wird vorgeschrieben, dass das MS Dynamics-Konto zuerst korrekt synchronisiert wird.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Leads: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * API-Dokumentation zum Synchronisieren von Leads: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. MS Dynamics-Opportunities mit Marketo synchronisieren.

   Sie müssen eine Marketo-Opportunity für die MS Dynamics-Opportunity upsertieren. Die Felder _externalOpportunityId_, _externalCompanyId_ und _externalSalesPersonId_ werden für das Upsert der Opportunity benötigt.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity-Objektfeld</strong></td> 
      <td><strong>MS Dynamics Opportunity-Objektfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei MS Dynamics Lead/Kontakt</td> 
      <td>Identifiziert den Marketo Opportunity-Datensatz für ein externes MS Dynamics Opportunity-Objekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung für MS Dynamics-Konto</td> 
      <td>Identifiziert das externe MS Dynamics-Kontoobjekt, zu dem diese Opportunity gehört. <br><br>Es ist erforderlich, dass das MS Dynamics-Konto zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Globale eindeutige Kennung ohne Berücksichtigung der Groß-/Kleinschreibung bei MS Dynamics Sales</td> 
      <td>Identifiziert das externe MS Dynamics-Verkaufsbenutzerobjekt, dem diese Opportunity gehört. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation zum Synchronisieren von Opportunities: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. MS Dynamics-Kontaktrollen mit Marketo synchronisieren.

   MS Dynamics-Kontaktrollen für eine MS Dynamics-Opportunity können dann über die Marketo-Opportunity-Rolle synchronisiert werden. Der Datensatz für die Opportunity-Rolle erfordert die Felder _externalOpportunityId_, _role_ und _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity-Rollenfeld</strong></td> 
      <td><strong>MS Dynamics-Kontaktrollenfeld</strong></td> 
      <td><strong>Beschreibung</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Globale eindeutige Kennung ohne Unterscheidung der Groß-/Kleinschreibung bei MS Dynamics-Opportunity</td> 
      <td>Identifiziert die Marketo-Opportunity-Rolle in einem externen MS Dynamics-Opportunity-Objekt.<br><br>Es wird vorgeschrieben, dass die MS Dynamics-Opportunity zuerst korrekt synchronisiert wird.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Nicht zutreffend, dies wäre eine Marketo Lead-ID.</td> 
      <td>Dies wäre die Marketo-Lead-ID des synchronisierten MS Dynamics-Kontakts.<br><br>Sobald der Kontakt in Marketo synchronisiert wurde, können Sie die eindeutige Kennung „MS Dynamics-Kontakt“ ohne Berücksichtigung der Groß-/Kleinschreibung“ als externePersonId verwenden und mit der Marketo-REST-API eine Abfrage für den Marketo-Lead durchführen.</td> 
     </tr> 
     <tr> 
      <td>Rolle</td> 
      <td>Das Rollenfeld für den MS Dynamics-Kontakt</td> 
      <td>Beschreibt die Rolle des Kontakts für diese Opportunity.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-Dokumentation für Opportunity: [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-Dokumentation zum Synchronisieren von Opportunities: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Letzten interessanten Moment/MSI-Bewertungsfelder mit MS Dynamics synchronisieren.

   Sobald Ihre MS Dynamics-Objekte korrekt mit Marketo synchronisiert wurden, können Sie die MSI-Funktionen nutzen. Die Felder für den letzten interessanten MSI-Moment/die letzte Bewertung werden in der REST-API für Leads angezeigt. Diese Felder werden von MSI berechnet und sind schreibgeschützt.

   Die Felder „Letzter interessanter Moment/letzte Bewertung“ eines Marketo-Leads müssen regelmäßig mithilfe des Lead-Endpunkts der REST-API mit MS Dynamics synchronisiert werden. Fragen Sie diesen Endpunkt für einen Marketo-Lead mit _externalPersonId_ als filterType ab und übergeben Sie die MS Dynamics-Lead-GUID als filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Sie können dann die Werte dieser Felder verwenden, um sie mit Ihrem MS Dynamics Lead/Kontakt-Objekt zu synchronisieren.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead-Feld</strong></td> 
      <td><strong>MS Dynamics Lead/Kontakt-Feld</strong></td> 
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

   * Dokumentation für die Lead-REST-API: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   Die ordnungsgemäße Verwendung der externen Felder ist der Schlüssel für eine erfolgreiche nicht-native Synchronisation. Wenn in einigen Ansichten keine Daten angezeigt werden, ist es wahrscheinlich, dass ein bestimmtes Feld nicht korrekt synchronisiert wurde. Wenn beispielsweise die Aktivitäten und interessanten Momente eines Leads beim Anzeigen im MSI-Widget unter seinem Konto nicht angezeigt werden, ist es wahrscheinlich, dass entweder das Unternehmen des Leads oder das Konto nicht korrekt synchronisiert wurde. Wenn Sie eine GET-Anfrage für diesen Lead ausführen und dabei die externen Felder angeben, können Sie überprüfen, ob der Lead korrekt synchronisiert wurde. Darüber hinaus muss die E-Mail für den externen Vertriebspersonal in Marketo mit der E-Mail für diesen Benutzer in MS Dynamics übereinstimmen. Daten werden möglicherweise nicht auf der Registerkarte Marketo in MS Dynamics angezeigt, wenn die E-Mails nicht übereinstimmen.
