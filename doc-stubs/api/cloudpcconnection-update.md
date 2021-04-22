---
title: "Update cloudPcConnection"
description: "Update the properties of a cloudPcConnection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cloudPcConnection
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [cloudPcConnection](../resources/cloudpcconnection.md) object.

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
PATCH /cloudPcConnections/{cloudPcConnectionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcConnection](../resources/cloudpcconnection.md) object.

The following table shows the properties that are required when you update the [cloudPcConnection](../resources/cloudpcconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|healthCheckStatus|String|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [cloudPcConnection](../resources/cloudpcconnection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cloudpcconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/cloudPcConnections/{cloudPcConnectionsId}
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.cloudPcConnection",
  "displayName": "String",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "healthCheckStatus": "String",
  "lastUpdated": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcConnection",
  "id": "85fb8067-8067-85fb-6780-fb856780fb85",
  "displayName": "String",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "healthCheckStatus": "String",
  "lastUpdated": "String (timestamp)"
}
```

