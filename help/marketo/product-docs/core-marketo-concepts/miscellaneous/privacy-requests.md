---
description: Datenschutzanfragen - Marketo-Dokumente - Produktdokumentation
title: Datenschutzanfragen
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 13%

---

# Datenschutzanfragen {#privacy-requests}

Dieses Dokument bietet einen Überblick über die Verwaltung individueller Datenschutzanfragen, die Sie über die Privacy Service-Benutzeroberfläche und die Privacy Service-API an Marketo Engage senden können.

>[!NOTE]
>
>Datenschutzanfragen, die über die Privacy Service-Benutzeroberfläche oder -API zum Marketo Engage übermittelt werden, gelten nur für Folgendes:
>
>* Marketo Engage-Benutzer, die sich beim Adobe Identity Management-System angemeldet haben
>
>**– oder –**
>
>* Marketo Engage-Anwender, die ein anderes Experience Cloud-Produkt verwenden, das sich bereits auf dem Adobe Identity Management-System befindet (z. B. RT-CDP, B2B und B2P Editions, Audience Manager).

Sie können individuelle Anfragen für den Zugriff auf und das Löschen von Verbraucherdaten von Marketo Engage auf zwei Arten stellen:

* Über die [Privacy Service-Benutzeroberfläche](https://privacyui.cloud.adobe.io/). Siehe die Dokumentation [hier](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=de){target="_blank"}.
* Über die Privacy Service-API. Siehe die Dokumentation [hier](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} und API-Informationen [hier](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

Der [Privacy Service ](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=de){target="_blank"} unterstützt zwei Anfragetypen: Datenzugriff und Datenlöschung.

Sehen wir uns an, wie Sie Zugriffs- und Löschanfragen erstellen können.

## Erforderliche Einrichtung zum Senden von Anfragen für Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Um Anfragen zum Zugreifen auf und Löschen von Daten für Marketo Engage zu stellen, ist Folgendes erforderlich:

1. Sie benötigen:

   a. Kennung der IMS-Organisation<br/>
b. E-Mail-Adresse der Person, die Sie bearbeiten möchten

   Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketing-Team oder der interne Adobe-Systemadministrator die IMS-Organisations-ID Ihres Unternehmens nicht kennt, wenden Sie sich unter `gdprsupport@adobe.com` an die Kundenunterstützung von Adobe. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

1. Im Privacy Service können Sie Zugriffs- und Löschanfragen an Marketo Engage senden und den Status vorhandener Anfragen überprüfen.

## Erforderliche Feldwerte beim Marketo Engage von JSON-Anfragen {#required-field-values-in-marketo-engage-json-requests}

„companyContexts“:

* &quot;namespace&quot;: **imsOrgID**
* „value“: `<Your IMS Org ID Value>`

&quot;users&quot;:

* &quot;action&quot;: entweder **Zugriff** oder **Löschen**
* „userIDs“:
   * „namespace“: **email**
   * „Typ“: **Standard**
   * „value“: `<Data Subject's Email Address>`

„Include“:

* **marketo** (das Adobe-Produkt, das für die Anfrage gilt)

„Verordnung“:

* **DSGVO**, **CCPA**, **PDPA**, **LGPD_BRA** oder **NZPA_NZL** (dies ist die Datenschutzverordnung, die für die Anfrage gilt)

## Beispiel 1: DSGVO-Löschanfrage {#gdpr-delete-request}

JSON-Anfrage

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

JSON-Antwort

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Beispiel 2: CCPA-Zugriffsanfrage {#ccpa-access-request}

JSON-Anfrage

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

JSON-Antwort

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[Datenschutzverwaltung](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
