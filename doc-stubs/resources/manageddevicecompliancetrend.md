---
title: "managedDeviceComplianceTrend resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceComplianceTrend resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedDeviceComplianceTrends](../api/manageddevicecompliancetrend-list.md)|[managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) collection|Get a list of the [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) objects and their properties.|
|[Create managedDeviceComplianceTrend](../api/manageddevicecompliancetrend-post-manageddevicecompliancetrends.md)|[managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md)|Create a new [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.|
|[Get managedDeviceComplianceTrend](../api/manageddevicecompliancetrend-get.md)|[managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md)|Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.|
|[Update managedDeviceComplianceTrend](../api/manageddevicecompliancetrend-update.md)|[managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md)|Update the properties of a [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.|
|[Delete managedDeviceComplianceTrend](../api/manageddevicecompliancetrend-delete.md)|None|Deletes a [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|configManagerDeviceCount|Int32|**TODO: Add Description**|
|countDateTime|String|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|inGracePeriodDeviceCount|Int32|**TODO: Add Description**|
|noncompliantDeviceCount|Int32|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceComplianceTrend",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```

