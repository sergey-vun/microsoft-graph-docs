---
title: "cloudPcConnection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudPcConnection resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cloudPcConnections](../api/cloudpcconnection-list.md)|[cloudPcConnection](../resources/cloudpcconnection.md) collection|Get a list of the [cloudPcConnection](../resources/cloudpcconnection.md) objects and their properties.|
|[Create cloudPcConnection](../api/cloudpcconnection-post-cloudpcconnections.md)|[cloudPcConnection](../resources/cloudpcconnection.md)|Create a new [cloudPcConnection](../resources/cloudpcconnection.md) object.|
|[Get cloudPcConnection](../api/cloudpcconnection-get.md)|[cloudPcConnection](../resources/cloudpcconnection.md)|Read the properties and relationships of a [cloudPcConnection](../resources/cloudpcconnection.md) object.|
|[Update cloudPcConnection](../api/cloudpcconnection-update.md)|[cloudPcConnection](../resources/cloudpcconnection.md)|Update the properties of a [cloudPcConnection](../resources/cloudpcconnection.md) object.|
|[Delete cloudPcConnection](../api/cloudpcconnection-delete.md)|None|Deletes a [cloudPcConnection](../resources/cloudpcconnection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|healthCheckStatus|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcConnection",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "healthCheckStatus": "String",
  "lastUpdated": "String (timestamp)"
}
```

