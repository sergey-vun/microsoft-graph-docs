---
title: "Create lambdaDefinition"
description: "Create a new lambdaDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create lambdaDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [lambdaDefinition](../resources/lambdadefinition.md) object.

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
POST ** Collection URI for microsoft.management.services.api.lambdaDefinition not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [lambdaDefinition](../resources/lambdadefinition.md) object.

The following table shows the properties that are required when you create the [lambdaDefinition](../resources/lambdadefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|type|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|value|String|**TODO: Add Description**|
|configuration|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [lambdaDefinition](../resources/lambdadefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_lambdadefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.lambdaDefinition not found
Content-Type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.management.services.api.lambdaDefinition",
  "type": "Integer",
  "value": "String",
  "configuration": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.lambdaDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.lambdaDefinition",
  "type": "Integer",
  "id": "8c60cf6a-cf6a-8c60-6acf-608c6acf608c",
  "value": "String",
  "configuration": "String"
}
```

