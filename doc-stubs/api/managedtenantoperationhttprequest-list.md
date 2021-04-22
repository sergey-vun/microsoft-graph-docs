---
title: "List managedTenantOperationHttpRequests"
description: "Get a list of the managedTenantOperationHttpRequest objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedTenantOperationHttpRequests
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) objects and their properties.

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
GET /managedTenantOperationHttpRequests
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

If successful, this method returns a `200 OK` response code and a collection of [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_managedtenantoperationhttprequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenantOperationHttpRequests
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.managedTenantOperationHttpRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.management.services.api.managedTenantOperationHttpRequest",
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
  ]
}
```

