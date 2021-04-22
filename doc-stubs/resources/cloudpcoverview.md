---
title: "cloudPcOverview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudPcOverview resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cloudPcOverviews](../api/cloudpcoverview-list.md)|[cloudPcOverview](../resources/cloudpcoverview.md) collection|Get a list of the [cloudPcOverview](../resources/cloudpcoverview.md) objects and their properties.|
|[Create cloudPcOverview](../api/cloudpcoverview-post-cloudpcsoverview.md)|[cloudPcOverview](../resources/cloudpcoverview.md)|Create a new [cloudPcOverview](../resources/cloudpcoverview.md) object.|
|[Get cloudPcOverview](../api/cloudpcoverview-get.md)|[cloudPcOverview](../resources/cloudpcoverview.md)|Read the properties and relationships of a [cloudPcOverview](../resources/cloudpcoverview.md) object.|
|[Update cloudPcOverview](../api/cloudpcoverview-update.md)|[cloudPcOverview](../resources/cloudpcoverview.md)|Update the properties of a [cloudPcOverview](../resources/cloudpcoverview.md) object.|
|[Delete cloudPcOverview](../api/cloudpcoverview-delete.md)|None|Deletes a [cloudPcOverview](../resources/cloudpcoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|cloudPcStatus_deprovisioning|Int32|**TODO: Add Description**|
|cloudPcStatus_failed|Int32|**TODO: Add Description**|
|cloudPcStatus_inGracePeriod|Int32|**TODO: Add Description**|
|cloudPcStatus_notProvisioned|Int32|**TODO: Add Description**|
|cloudPcStatus_provisioned|Int32|**TODO: Add Description**|
|cloudPcStatus_provisioning|Int32|**TODO: Add Description**|
|cloudPcStatus_total|Int32|**TODO: Add Description**|
|cloudPcStatus_unknown|Int32|**TODO: Add Description**|
|cloudPcStatus_upgrading|Int32|**TODO: Add Description**|
|connectionStatus_failed|Int32|**TODO: Add Description**|
|connectionStatus_passed|Int32|**TODO: Add Description**|
|connectionStatus_pending|Int32|**TODO: Add Description**|
|connectionStatus_running|Int32|**TODO: Add Description**|
|connectionStatus_total|Int32|**TODO: Add Description**|
|connectionStatus_unkownFutureValue|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOverview",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOverview",
  "id": "String (identifier)",
  "organizationDisplayName": "String",
  "cloudPcStatus_total": "Integer",
  "cloudPcStatus_notProvisioned": "Integer",
  "cloudPcStatus_provisioning": "Integer",
  "cloudPcStatus_provisioned": "Integer",
  "cloudPcStatus_upgrading": "Integer",
  "cloudPcStatus_inGracePeriod": "Integer",
  "cloudPcStatus_deprovisioning": "Integer",
  "cloudPcStatus_failed": "Integer",
  "cloudPcStatus_unknown": "Integer",
  "connectionStatus_total": "Integer",
  "connectionStatus_pending": "Integer",
  "connectionStatus_running": "Integer",
  "connectionStatus_passed": "Integer",
  "connectionStatus_failed": "Integer",
  "connectionStatus_unkownFutureValue": "Integer",
  "lastUpdated": "String (timestamp)"
}
```

