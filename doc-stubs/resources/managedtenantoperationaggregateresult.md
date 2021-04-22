---
title: "managedTenantOperationAggregateResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantOperationAggregateResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|exception|String|**TODO: Add Description**|
|executionInfo|String|**TODO: Add Description**|
|isComplete|Boolean|**TODO: Add Description**|
|isSuccess|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|result|String collection|**TODO: Add Description**|
|tenantExceptions|[tenantException](../resources/tenantexception.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenantOperationAggregateResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantOperationAggregateResult",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isSuccess": "Boolean",
  "exception": "String",
  "executionInfo": "String",
  "isComplete": "Boolean",
  "tenantExceptions": [
    {
      "@odata.type": "microsoft.graph.tenantException"
    }
  ],
  "result": [
    "String"
  ]
}
```

