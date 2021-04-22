---
title: "managedTenantOperationResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantOperationResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedTenantOperationResults](../api/managedtenantoperationresult-list.md)|[managedTenantOperationResult](../resources/managedtenantoperationresult.md) collection|Get a list of the [managedTenantOperationResult](../resources/managedtenantoperationresult.md) objects and their properties.|
|[Create managedTenantOperationResult](../api/managedtenantoperationresult-post-managedtenantoperationresults.md)|[managedTenantOperationResult](../resources/managedtenantoperationresult.md)|Create a new [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.|
|[Get managedTenantOperationResult](../api/managedtenantoperationresult-get.md)|[managedTenantOperationResult](../resources/managedtenantoperationresult.md)|Read the properties and relationships of a [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.|
|[Update managedTenantOperationResult](../api/managedtenantoperationresult-update.md)|[managedTenantOperationResult](../resources/managedtenantoperationresult.md)|Update the properties of a [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.|
|[Delete managedTenantOperationResult](../api/managedtenantoperationresult-delete.md)|None|Deletes a [managedTenantOperationResult](../resources/managedtenantoperationresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|exception|String|**TODO: Add Description**|
|executionInfo|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isSuccess|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|managedTenantOperationId|String|**TODO: Add Description**|
|partnerTenantId|Guid|**TODO: Add Description**|
|partnerUserId|Guid|**TODO: Add Description**|
|requestId|Guid|**TODO: Add Description**|
|result|String collection|**TODO: Add Description**|
|targetTenantId|Guid|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenantOperationResult",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantOperationResult",
  "id": "String (identifier)",
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

