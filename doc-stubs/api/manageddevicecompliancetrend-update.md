---
title: "Update managedDeviceComplianceTrend"
description: "Update the properties of a managedDeviceComplianceTrend object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedDeviceComplianceTrend
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /managedDeviceComplianceTrends/{managedDeviceComplianceTrendsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object.

The following table shows the properties that are required when you update the [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|noncompliantDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|inGracePeriodDeviceCount|Int32|**TODO: Add Description**|
|configManagerDeviceCount|Int32|**TODO: Add Description**|
|countDateTime|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedDeviceComplianceTrend](../resources/manageddevicecompliancetrend.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_manageddevicecompliancetrend"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/managedDeviceComplianceTrends/{managedDeviceComplianceTrendsId}
Content-Type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.managedDeviceComplianceTrend",
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


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedDeviceComplianceTrend",
  "id": "8e84db46-db46-8e84-46db-848e46db848e",
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

