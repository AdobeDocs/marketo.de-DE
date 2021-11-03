---
description: Datenschutzanfragen - Marketo-Dokumente - Produktdokumentation
title: Datenschutzanfragen
source-git-commit: 17e68ea00647dbfd98fde94827eb300804944511
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Datenschutzanfragen {#privacy-requests}

Dieses Dokument bietet einen Überblick über die Verwaltung individueller Datenschutzanfragen, die Sie über die Privacy Service-Benutzeroberfläche und die **Privacy Service-API**.

Sie können individuelle Anfragen zum Zugriff auf und zum Löschen von Verbraucherdaten aus Marketo Engage auf zwei Arten senden:

* Durch die [Privacy Service-Benutzeroberfläche](https://privacyui.cloud.adobe.io/). Weitere Informationen finden Sie in der Dokumentation [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* Durch die **Privacy Service-API**. Weitere Informationen finden Sie in der Dokumentation [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) und die API-Referenz [here](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

Die [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) unterstützt zwei Arten von Anforderungen: Datenzugriff und Datenlöschung.

Hinweis: Datenschutzanfragen, die über die Privacy Service-Benutzeroberfläche oder -API zum Marketo Engage gesendet werden, gelten nur für Kunden mit Marketo Engage + RT-CDP, B2B- und B2P-Editionen.

Sehen wir uns an, wie Sie Zugriffs- und Löschanfragen erstellen können.

## Erforderliche Einrichtung zum Senden von Anforderungen an Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Um Anfragen zum Zugreifen auf und Löschen von Daten für Marketo Engage zu stellen, müssen Sie:

1. Identifizieren Sie Folgendes:

   a. Kennung der IMS-Organisation<br/>
b. E-Mail-Adresse der Person, auf die Sie reagieren möchten

   Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketing-Team oder Ihr Systemadministrator des internen Adobe die IMS-Organisations-ID Ihres Unternehmens nicht kennen, wenden Sie sich an die Kundenunterstützung von Adobe unter gdprsupport@adobe.com. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

1. In Privacy Service können Sie Zugriffs- und Löschanfragen an Marketo Engage senden und den Status vorhandener Anfragen überprüfen.

## Erforderliche Feldwerte in Marketo Engage-JSON-Anforderungen {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* “Wert”: `<Your IMS Org ID Value>`

“Benutzer”:

* &quot;key&quot;: `<Your Request Tracking Key>`   (optional)
* &quot;action&quot;: entweder **access** oder **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * “Wert”: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (das Adobe-Produkt, das für die Anfrage gilt)

&quot;Verordnung&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd** oder **nzpa**  (die Datenschutzverordnung, die für die Anfrage gilt)

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
      "key": "AAGDPRO1", 
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
          "key": "AAGDPRO1",
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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
      "key": "AAGDPRO1",
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
      "jobId": " 3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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
