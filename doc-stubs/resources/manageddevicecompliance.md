---
title: "managedDeviceCompliance resource type"
description: "**TODO: Add Description**"
author: isaiahwilliams
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceCompliance resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedDeviceCompliances](../api/manageddevicecompliance-list.md)|[managedDeviceCompliance](../resources/manageddevicecompliance.md) collection|Get a list of the [managedDeviceCompliance](../resources/manageddevicecompliance.md) objects and their properties.|
|[Get managedDeviceCompliance](../api/manageddevicecompliance-get.md)|[managedDeviceCompliance](../resources/manageddevicecompliance.md)|Read the properties and relationships of a [managedDeviceCompliance](../resources/manageddevicecompliance.md) object.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
|complianceStatus|String|**TODO: Add Description**|
|deviceType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|inGracePeriodUntilDateTime|DateTimeOffset|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|osDescription|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|ownerType|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCompliance",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "complianceStatus": "String",
  "osDescription": "String",
  "osVersion": "String",
  "lastSyncDateTime": "String (timestamp)",
  "ownerType": "String",
  "model": "String",
  "manufacturer": "String",
  "inGracePeriodUntilDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)",
  "deviceType": "String"
}
```

