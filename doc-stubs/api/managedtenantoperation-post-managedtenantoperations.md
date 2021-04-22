---
title: "Create managedTenantOperation"
description: "Create a new managedTenantOperation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedTenantOperation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [managedTenantOperation](../resources/managedtenantoperation.md) object.

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
POST /managedTenantOperations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantOperation](../resources/managedtenantoperation.md) object.

The following table shows the properties that are required when you create the [managedTenantOperation](../resources/managedtenantoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|result|[managedTenantOperationAggregateResult](../resources/managedtenantoperationaggregateresult.md)|**TODO: Add Description**|
|target|[managedTenantOperationTarget](../resources/managedtenantoperationtarget.md)|**TODO: Add Description**|
|operationDefinition|[managedTenantOperationDefinition](../resources/managedtenantoperationdefinition.md)|**TODO: Add Description**|
|aggregationDefinition|[managedTenantOperationDefinition](../resources/managedtenantoperationdefinition.md)|**TODO: Add Description**|
|credentials|[managedTenantOperationCredentials](../resources/managedtenantoperationcredentials.md)|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|partnerTenantId|Guid|**TODO: Add Description**|
|partnerUserId|Guid|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|requestId|Guid|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedTenantOperation](../resources/managedtenantoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedtenantoperation_from_managedtenantoperations"
}
-->
``` http
POST https://graph.microsoft.com/beta/managedTenantOperations
Content-Type: application/json
Content-length: 731

{
  "@odata.type": "#microsoft.management.services.api.managedTenantOperation",
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
  "partnerTenantId": "Guid",
  "partnerUserId": "Guid",
  "name": "String",
  "description": "String",
  "requestId": "Guid"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedTenantOperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```

