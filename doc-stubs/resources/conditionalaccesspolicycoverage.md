---
title: "conditionalAccessPolicyCoverage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessPolicyCoverage resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List conditionalAccessPolicyCoverages](../api/conditionalaccesspolicycoverage-list.md)|[conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) collection|Get a list of the [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) objects and their properties.|
|[Create conditionalAccessPolicyCoverage](../api/conditionalaccesspolicycoverage-post-conditionalaccesspolicycoverages.md)|[conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md)|Create a new [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.|
|[Get conditionalAccessPolicyCoverage](../api/conditionalaccesspolicycoverage-get.md)|[conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md)|Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.|
|[Update conditionalAccessPolicyCoverage](../api/conditionalaccesspolicycoverage-update.md)|[conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md)|Update the properties of a [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.|
|[Delete conditionalAccessPolicyCoverage](../api/conditionalaccesspolicycoverage-delete.md)|None|Deletes a [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conditionalAccessPolicyState|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|latestPolicyModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|requiresDeviceCompliance|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conditionalAccessPolicyCoverage",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```

