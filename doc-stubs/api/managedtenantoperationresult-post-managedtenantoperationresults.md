---
title: "Create managedTenantOperationResult"
description: "Create a new managedTenantOperationResult object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedTenantOperationResult
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.

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
POST /managedTenantOperationResults
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.

The following table shows the properties that are required when you create the [managedTenantOperationResult](../resources/managedtenantoperationresult.md).

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
|isSuccess|Boolean|**TODO: Add Description**|
|exception|String|**TODO: Add Description**|
|executionInfo|String|**TODO: Add Description**|
|result|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedtenantoperationresult_from_managedtenantoperationresults"
}
-->
``` http
POST https://graph.microsoft.com/beta/managedTenantOperationResults
Content-Type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.management.services.api.managedTenantOperationResult",
  "partnerTenantId": "Guid",
  "partnerUserId": "Guid",
  "targetTenantId": "Guid",
  "managedTenantOperationId": "String",
  "requestId": "Guid",
  "isSuccess": "Boolean",
  "exception": "String",
  "executionInfo": "String",
  "result": [
    "String"
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedTenantOperationResult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.managedTenantOperationResult",
  "id": "c1448cfc-8cfc-c144-fc8c-44c1fc8c44c1",
  "partnerTenantId": "Guid",
  "partnerUserId": "Guid",
  "targetTenantId": "Guid",
  "managedTenantOperationId": "String",
  "requestId": "Guid",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isSuccess": "Boolean",
  "exception": "String",
  "executionInfo": "String",
  "result": [
    "String"
  ]
}
```

