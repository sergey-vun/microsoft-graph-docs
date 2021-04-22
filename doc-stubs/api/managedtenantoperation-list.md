---
title: "List managedTenantOperations"
description: "Get a list of the managedTenantOperation objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedTenantOperations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [managedTenantOperation](../resources/managedtenantoperation.md) objects and their properties.

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
GET /managedTenantOperations
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

If successful, this method returns a `200 OK` response code and a collection of [managedTenantOperation](../resources/managedtenantoperation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_managedtenantoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenantOperations
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.managedTenantOperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.management.services.api.managedTenantOperation",
      "id": "7b7246f6-46f6-7b72-f646-727bf646727b",
      "result": {
        "@odata.type": "microsoft.graph.managedTenantOperationAggregateResult"
      },
      "target": {
        "@odata.type": "microsoft.graph.managedTenantOperationTarget"
      },
      "operationDefinition": {
        "@odata.type": "microsoft.graph.managedTenantOperationDefinition"
      },
      "aggregationDefinition": {
        "@odata.type": "microsoft.graph.managedTenantOperationDefinition"
      },
      "credentials": {
        "@odata.type": "microsoft.graph.managedTenantOperationCredentials"
      },
      "status": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "partnerTenantId": "Guid",
      "partnerUserId": "Guid",
      "name": "String",
      "description": "String",
      "requestId": "Guid"
    }
  ]
}
```

