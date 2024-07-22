---
description: Datenschutzanfragen - Marketo-Dokumente - Produktdokumentation
title: Datenschutzanfragen
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Datenschutzanfragen {#privacy-requests}

Dieses Dokument bietet einen Überblick über die Verwaltung individueller Datenschutzanfragen, die Sie über die Privacy Service-Benutzeroberfläche und die Privacy Service-API an Marketo Engage senden können.

>[!NOTE]
>
>Datenschutzanfragen, die über die Privacy Service-Benutzeroberfläche oder -API zum Marketo Engage gesendet werden, gelten nur für Folgendes:
>
>* Marketo Engage-Benutzer, die an Adobe Identity Management System angeschlossen sind
>
>**– oder –**
>
>* Marketo Engage-Anwender, die ein anderes Experience Cloud-Produkt verwenden, das bereits auf dem Adobe-Identity Management-System installiert ist (z. B. RT-CDP, B2B und B2P Editions, Audience Manager).

Sie können individuelle Anfragen zum Zugriff auf und zum Löschen von Verbraucherdaten aus dem Marketo Engage auf zwei Arten senden:

* Über die [Privacy Service-Benutzeroberfläche](https://privacyui.cloud.adobe.io/). Weitere Informationen finden Sie in der Dokumentation [hier](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=de){target="_blank"} .
* Über die Privacy Service-API. Die Dokumentation [hier](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} und API-Informationen [hier](https://developer.adobe.com/experience-platform-apis/){target="_blank"} finden Sie in der Dokumentation.

Der [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target="_blank"} unterstützt zwei Arten von Anforderungen: Datenzugriff und Datenlöschung.

Im Folgenden wird beschrieben, wie Sie Zugriffs- und Löschanfragen erstellen können.

## Erforderliche Einrichtung zum Senden von Anfragen für Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Um Anfragen zum Zugreifen auf und Löschen von Daten für Marketo Engage zu stellen, müssen Sie:

1. Identifizieren Sie Folgendes:

   a. IMS-Organisations-ID<br/>
b. E-Mail-Adresse der Person, auf die Sie reagieren möchten

   Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketing-Team oder der interne Adobe-Systemadministrator die IMS-Organisations-ID Ihres Unternehmens nicht kennen, wenden Sie sich unter `gdprsupport@adobe.com` an die Adobe-Kundenunterstützung. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

1. In Privacy Service können Sie Zugriffs- und Löschanfragen an Marketo Engage senden und den Status vorhandener Anfragen überprüfen.

## Erforderliche Feldwerte in Marketo Engage-JSON-Anforderungen {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot;:

* &quot;action&quot;: entweder **access** oder **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject's Email Address>`

&quot;include&quot;:

* **marketo** (das Adobe-Produkt, das für die Anforderung gilt)

&quot;Verordnung&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** oder **nzpa_nzl** (die Datenschutzverordnung, die für die Anfrage gilt)

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
