---
title: "managedTenantOperationHttpRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantOperationHttpRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedTenantOperationHttpRequests](../api/managedtenantoperationhttprequest-list.md)|[managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) collection|Get a list of the [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) objects and their properties.|
|[Create managedTenantOperationHttpRequest](../api/managedtenantoperationhttprequest-post-managedtenantoperationhttprequests.md)|[managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md)|Create a new [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.|
|[Get managedTenantOperationHttpRequest](../api/managedtenantoperationhttprequest-get.md)|[managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md)|Read the properties and relationships of a [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.|
|[Update managedTenantOperationHttpRequest](../api/managedtenantoperationhttprequest-update.md)|[managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md)|Update the properties of a [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.|
|[Delete managedTenantOperationHttpRequest](../api/managedtenantoperationhttprequest-delete.md)|None|Deletes a [managedTenantOperationHttpRequest](../resources/managedtenantoperationhttprequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attempt|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|managedTenantOperationId|String|**TODO: Add Description**|
|partnerTenantId|Guid|**TODO: Add Description**|
|partnerUserId|Guid|**TODO: Add Description**|
|request|[httpRequest](../resources/httprequest.md)|**TODO: Add Description**|
|requestId|Guid|**TODO: Add Description**|
|response|[httpResponse](../resources/httpresponse.md)|**TODO: Add Description**|
|statusCode|Int32|**TODO: Add Description**|
|targetTenantId|Guid|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenantOperationHttpRequest",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantOperationHttpRequest",
  "id": "String (identifier)",
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

