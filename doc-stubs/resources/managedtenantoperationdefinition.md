---
title: "managedTenantOperationDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantOperationDefinition resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failOnFirstError|Boolean|**TODO: Add Description**|
|logLevel|logLevel|**TODO: Add Description**. Possible values are: `none`, `summary`, `full`.|
|value|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|lambdaDefinitions|[lambdaDefinition](../resources/lambdadefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenantOperationDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantOperationDefinition",
  "value": "String",
  "logLevel": "String",
  "failOnFirstError": "Boolean"
}
```

