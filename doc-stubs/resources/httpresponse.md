---
title: "httpResponse resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# httpResponse resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|body|String|**TODO: Add Description**|
|headers|[httpHeader](../resources/httpheader.md) collection|**TODO: Add Description**|
|status|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.httpResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.httpResponse",
  "status": "Integer",
  "body": "String",
  "headers": [
    {
      "@odata.type": "microsoft.graph.httpHeader"
    }
  ]
}
```

