---
title: "managedTenantOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantOperation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedTenantOperations](../api/managedtenantoperation-list.md)|[managedTenantOperation](../resources/managedtenantoperation.md) collection|Get a list of the [managedTenantOperation](../resources/managedtenantoperation.md) objects and their properties.|
|[Create managedTenantOperation](../api/managedtenantoperation-post-managedtenantoperations.md)|[managedTenantOperation](../resources/managedtenantoperation.md)|Create a new [managedTenantOperation](../resources/managedtenantoperation.md) object.|
|[Get managedTenantOperation](../api/managedtenantoperation-get.md)|[managedTenantOperation](../resources/managedtenantoperation.md)|Read the properties and relationships of a [managedTenantOperation](../resources/managedtenantoperation.md) object.|
|[Update managedTenantOperation](../api/managedtenantoperation-update.md)|[managedTenantOperation](../resources/managedtenantoperation.md)|Update the properties of a [managedTenantOperation](../resources/managedtenantoperation.md) object.|
|[Delete managedTenantOperation](../api/managedtenantoperation-delete.md)|None|Deletes a [managedTenantOperation](../resources/managedtenantoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregationDefinition|[managedTenantOperationDefinition](../resources/managedtenantoperationdefinition.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|credentials|[managedTenantOperationCredentials](../resources/managedtenantoperationcredentials.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|operationDefinition|[managedTenantOperationDefinition](../resources/managedtenantoperationdefinition.md)|**TODO: Add Description**|
|partnerTenantId|Guid|**TODO: Add Description**|
|partnerUserId|Guid|**TODO: Add Description**|
|requestId|Guid|**TODO: Add Description**|
|result|[managedTenantOperationAggregateResult](../resources/managedtenantoperationaggregateresult.md)|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|target|[managedTenantOperationTarget](../resources/managedtenantoperationtarget.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenantOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantOperation",
  "id": "String (identifier)",
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

