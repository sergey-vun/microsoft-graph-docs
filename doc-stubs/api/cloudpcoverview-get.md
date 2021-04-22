---
title: "Get cloudPcOverview"
description: "Read the properties and relationships of a cloudPcOverview object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get cloudPcOverview
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [cloudPcOverview](../resources/cloudpcoverview.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /cloudPcsOverview/{cloudPcsOverviewId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [cloudPcOverview](../resources/cloudpcoverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/cloudPcsOverview/{cloudPcsOverviewId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.cloudPcOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.management.services.api.cloudPcOverview",
    "id": "0b8d8da2-8da2-0b8d-a28d-8d0ba28d8d0b",
    "organizationDisplayName": "String",
    "cloudPcStatus_total": "Integer",
    "cloudPcStatus_notProvisioned": "Integer",
    "cloudPcStatus_provisioning": "Integer",
    "cloudPcStatus_provisioned": "Integer",
    "cloudPcStatus_upgrading": "Integer",
    "cloudPcStatus_inGracePeriod": "Integer",
    "cloudPcStatus_deprovisioning": "Integer",
    "cloudPcStatus_failed": "Integer",
    "cloudPcStatus_unknown": "Integer",
    "connectionStatus_total": "Integer",
    "connectionStatus_pending": "Integer",
    "connectionStatus_running": "Integer",
    "connectionStatus_passed": "Integer",
    "connectionStatus_failed": "Integer",
    "connectionStatus_unkownFutureValue": "Integer",
    "lastUpdated": "String (timestamp)"
  }
}
```

