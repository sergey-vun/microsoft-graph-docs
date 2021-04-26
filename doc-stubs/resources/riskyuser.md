---
title: "riskyUser resource type"
description: "**TODO: Add Description**"
author: "isaiahwilliams"
localization_priority: Normal
ms.prod: "microsoft365-lighthouse"
doc_type: resourcePageType
---

# riskyUser resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) collection|Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.|
|[Get riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|riskDetail|String|**TODO: Add Description**|
|riskLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|riskLevel|String|**TODO: Add Description**|
|riskState|String|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

