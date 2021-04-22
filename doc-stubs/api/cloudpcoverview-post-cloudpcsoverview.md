---
title: "Create cloudPcOverview"
description: "Create a new cloudPcOverview object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cloudPcOverview
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [cloudPcOverview](../resources/cloudpcoverview.md) object.

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
POST /cloudPcsOverview
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcOverview](../resources/cloudpcoverview.md) object.

The following table shows the properties that are required when you create the [cloudPcOverview](../resources/cloudpcoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|cloudPcStatus_total|Int32|**TODO: Add Description**|
|cloudPcStatus_notProvisioned|Int32|**TODO: Add Description**|
|cloudPcStatus_provisioning|Int32|**TODO: Add Description**|
|cloudPcStatus_provisioned|Int32|**TODO: Add Description**|
|cloudPcStatus_upgrading|Int32|**TODO: Add Description**|
|cloudPcStatus_inGracePeriod|Int32|**TODO: Add Description**|
|cloudPcStatus_deprovisioning|Int32|**TODO: Add Description**|
|cloudPcStatus_failed|Int32|**TODO: Add Description**|
|cloudPcStatus_unknown|Int32|**TODO: Add Description**|
|connectionStatus_total|Int32|**TODO: Add Description**|
|connectionStatus_pending|Int32|**TODO: Add Description**|
|connectionStatus_running|Int32|**TODO: Add Description**|
|connectionStatus_passed|Int32|**TODO: Add Description**|
|connectionStatus_failed|Int32|**TODO: Add Description**|
|connectionStatus_unkownFutureValue|Int32|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [cloudPcOverview](../resources/cloudpcoverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_cloudpcoverview_from_cloudpcsoverview"
}
-->
``` http
POST https://graph.microsoft.com/beta/cloudPcsOverview
Content-Type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.management.services.api.cloudPcOverview",
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
HTTP/1.1 201 Created
Content-Type: application/json

{
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
```

