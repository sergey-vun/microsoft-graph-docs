---
title: "cloudPcDevice resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudPcDevice resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cloudPcDevices](../api/cloudpcdevice-list.md)|[cloudPcDevice](../resources/cloudpcdevice.md) collection|Get a list of the [cloudPcDevice](../resources/cloudpcdevice.md) objects and their properties.|
|[Create cloudPcDevice](../api/cloudpcdevice-post-cloudpcdevices.md)|[cloudPcDevice](../resources/cloudpcdevice.md)|Create a new [cloudPcDevice](../resources/cloudpcdevice.md) object.|
|[Get cloudPcDevice](../api/cloudpcdevice-get.md)|[cloudPcDevice](../resources/cloudpcdevice.md)|Read the properties and relationships of a [cloudPcDevice](../resources/cloudpcdevice.md) object.|
|[Update cloudPcDevice](../api/cloudpcdevice-update.md)|[cloudPcDevice](../resources/cloudpcdevice.md)|Update the properties of a [cloudPcDevice](../resources/cloudpcdevice.md) object.|
|[Delete cloudPcDevice](../api/cloudpcdevice-delete.md)|None|Deletes a [cloudPcDevice](../resources/cloudpcdevice.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|policyId|String|**TODO: Add Description**|
|servicePlanName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDevice",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDevice",
  "id": "String (identifier)",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "displayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "status": "String",
  "lastUpdated": "String (timestamp)",
  "policyId": "String"
}
```

