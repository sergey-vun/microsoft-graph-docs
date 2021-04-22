---
title: "Update managedTenantOperationHttpRequest"
description: "Update the properties of a managedTenantOperationHttpRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedTenantOperationHttpRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.

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
PATCH /managedTenantOperationHttpRequests/{managedTenantOperationHttpRequestsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.

The following table shows the properties that are required when you update the [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|partnerTenantId|Guid|**TODO: Add Description**|
|partnerUserId|Guid|**TODO: Add Description**|
|targetTenantId|Guid|**TODO: Add Description**|
|managedTenantOperationId|String|**TODO: Add Description**|
|requestId|Guid|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|attempt|Int32|**TODO: Add Description**|
|statusCode|Int32|**TODO: Add Description**|
|request|[httpRequest](../resources/httprequest.md)|**TODO: Add Description**|
|response|[httpResponse](../resources/httpresponse.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedtenantoperationhttprequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/managedTenantOperationHttpRequests/{managedTenantOperationHttpRequestsId}
Content-Type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.managedTenantOperationHttpRequest",
  "partnerTenantId": "Guid",
  "partnerUserId": "Guid",
  "targetTenantId": "Guid",
  "managedTenantOperationId": "String",
  "requestId": "Guid",
  "attempt": "Integer",
  "statusCode": "Integer",
  "request": {
    "@odata.type": "microsoft.graph.httpRequest"
  },
  "response": {
    "@odata.type": "microsoft.graph.httpResponse"
  }
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
  "@odata.type": "#microsoft.graph.managedTenantOperationHttpRequest",
  "id": "911c203c-203c-911c-3c20-1c913c201c91",
  "partnerTenantId": "Guid",
  "partnerUserId": "Guid",
  "targetTenantId": "Guid",
  "managedTenantOperationId": "String",
  "requestId": "Guid",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "attempt": "Integer",
  "statusCode": "Integer",
  "request": {
    "@odata.type": "microsoft.graph.httpRequest"
  },
  "response": {
    "@odata.type": "microsoft.graph.httpResponse"
  }
}
```

