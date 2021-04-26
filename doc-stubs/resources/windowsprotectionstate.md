---
title: "windowsProtectionState resource type"
description: "**TODO: Add Description**"
author: "isaiahwilliams"
localization_priority: Normal
ms.prod: "microsoft365-lighthouse"
doc_type: resourcePageType
---

# windowsProtectionState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsProtectionStates](../api/windowsprotectionstate-list.md)|[windowsProtectionState](../resources/windowsprotectionstate.md) collection|Get a list of the [windowsProtectionState](../resources/windowsprotectionstate.md) objects and their properties.|
|[Get windowsProtectionState](../api/windowsprotectionstate-get.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Read the properties and relationships of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|antiMalwareVersion|String|**TODO: Add Description**|
|attentionRequired|Boolean|**TODO: Add Description**|
|deviceDeleted|Boolean|**TODO: Add Description**|
|devicePropertiesRefreshTime|DateTimeOffset|**TODO: Add Description**|
|engineVersion|String|**TODO: Add Description**|
|fullScanOverdue|Boolean|**TODO: Add Description**|
|fullScanRequired|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastFullScanDateTime|DateTimeOffset|**TODO: Add Description**|
|lastFullScanSignatureVersion|String|**TODO: Add Description**|
|lastQuickScanDateTime|DateTimeOffset|**TODO: Add Description**|
|lastQuickScanSignatureVersion|String|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastReportedDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareProtectionEnabled|Boolean|**TODO: Add Description**|
|managedDeviceHealthState|String|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|networkInspectionSystemEnabled|Boolean|**TODO: Add Description**|
|quickScanOverdue|Boolean|**TODO: Add Description**|
|realTimeProtectionEnabled|Boolean|**TODO: Add Description**|
|rebootRequired|Boolean|**TODO: Add Description**|
|signatureUpdateOverdue|Boolean|**TODO: Add Description**|
|signatureVersion|String|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "malwareProtectionEnabled": "Boolean",
  "managedDeviceHealthState": "String",
  "realTimeProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "fullScanOverdue": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "rebootRequired": "Boolean",
  "attentionRequired": "Boolean",
  "fullScanRequired": "Boolean",
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)",
  "devicePropertiesRefreshTime": "String (timestamp)",
  "deviceDeleted": "Boolean",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

