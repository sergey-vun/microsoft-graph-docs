---
title: "deviceCompliancePolicySettingStateSummary resource type"
description: "**TODO: Add Description**"
author: "isaiahwilliams"
localization_priority: Normal
ms.prod: "microsoft365-lighthouse"
doc_type: resourcePageType
---

# deviceCompliancePolicySettingStateSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceCompliancePolicySettingStateSummaries](../api/devicecompliancepolicysettingstatesummary-list.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) collection|Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) objects and their properties.|
|[Get deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|failedDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|intuneAccountId|String|**TODO: Add Description**|
|intuneSettingId|String|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|pendingDeviceCount|Int32|**TODO: Add Description**|
|policyType|String|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|succeededDeviceCount|Int32|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "intuneAccountId": "String",
  "intuneSettingId": "String",
  "policyType": "String",
  "settingName": "String",
  "pendingDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "succeededDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

