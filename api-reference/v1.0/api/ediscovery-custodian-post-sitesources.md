---
title: "Create custodian siteSource"
description: "Create a new custodian siteSource object."
author: "mahage-msft"
ms.localizationpriority: medium
ms.prod: "ediscovery"
doc_type: apiPageType
---

# Create custodian siteSource

Namespace: microsoft.graph.ediscovery

Create a new custodian [siteSource](../resources/ediscovery-sitesource.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.

The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).

|Property|Type|Description|
|:---|:---|:---|
|site|String|URL of the site; for example, `https://contoso.sharepoint.com/sites/HumanResources`.|

## Response

If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_sitesource_from__1"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/custodians/8904528fef4d4578b44f71a80188f400/siteSources
Content-Type: application/json
Content-length: 179

{
    "site": {
        "webUrl": "https://contoso.sharepoint.com/sites/HumanResources"
    }
}

```

---

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#compliance/ediscovery/cases('15d80234-8320-4f10-96d0-d98d53ffdfc9')/custodians('8904528fef4d4578b44f71a80188f400')/siteSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/sites/2493b4eb-1a48-4cac-b0d0-aad05e6b9df0",
    "displayName": "Human resources site",
    "createdDateTime": "2021-08-10T18:25:48.6441363Z",
    "id": "42393244-3838-4636-3437-453030334136",
    "createdBy": {
        "user": {
            "id": "798d8d23-2087-4e03-912e-c0d9db5cb5d2",
            "displayName": null
        }
    }
}
```