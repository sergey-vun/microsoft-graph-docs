---
title: "aggregatedPolicyCompliance resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# aggregatedPolicyCompliance resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List aggregatedPolicyCompliances](../api/aggregatedpolicycompliance-list.md)|[aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) collection|Get a list of the [aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) objects and their properties.|
|[Get aggregatedPolicyCompliance](../api/aggregatedpolicycompliance-get.md)|[aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md)|Read the properties and relationships of an [aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliancePolicyId|String|**TODO: Add Description**|
|compliancePolicyName|String|**TODO: Add Description**|
|compliancePolicyPlatform|String|**TODO: Add Description**|
|compliancePolicyType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|numberOfCompliantDevices|Int64|**TODO: Add Description**|
|numberOfErrorDevices|Int64|**TODO: Add Description**|
|numberOfNonCompliantDevices|Int64|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|policyModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aggregatedPolicyCompliance",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

