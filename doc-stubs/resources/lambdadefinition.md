---
title: "lambdaDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# lambdaDefinition resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List lambdaDefinitions](../api/lambdadefinition-list.md)|[lambdaDefinition](../resources/lambdadefinition.md) collection|Get a list of the [lambdaDefinition](../resources/lambdadefinition.md) objects and their properties.|
|[Create lambdaDefinition](../api/lambdadefinition-create.md)|[lambdaDefinition](../resources/lambdadefinition.md)|Create a new [lambdaDefinition](../resources/lambdadefinition.md) object.|
|[Get lambdaDefinition](../api/lambdadefinition-get.md)|[lambdaDefinition](../resources/lambdadefinition.md)|Read the properties and relationships of a [lambdaDefinition](../resources/lambdadefinition.md) object.|
|[Update lambdaDefinition](../api/lambdadefinition-update.md)|[lambdaDefinition](../resources/lambdadefinition.md)|Update the properties of a [lambdaDefinition](../resources/lambdadefinition.md) object.|
|[Delete lambdaDefinition](../api/lambdadefinition-delete.md)|None|Deletes a [lambdaDefinition](../resources/lambdadefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|type|Int32|**TODO: Add Description**|
|value|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.lambdaDefinition",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.lambdaDefinition",
  "type": "Integer",
  "id": "String (identifier)",
  "value": "String",
  "configuration": "String"
}
```

