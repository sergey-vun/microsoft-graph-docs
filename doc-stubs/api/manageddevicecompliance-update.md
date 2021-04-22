---
title: "Update managedDeviceCompliance"
description: "Update the properties of a managedDeviceCompliance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedDeviceCompliance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [managedDeviceCompliance](../resources/manageddevicecompliance.md) object.

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
PATCH /managedDeviceCompliances/{managedDeviceCompliancesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceCompliance](../resources/manageddevicecompliance.md) object.

The following table shows the properties that are required when you update the [managedDeviceCompliance](../resources/manageddevicecompliance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|complianceStatus|String|**TODO: Add Description**|
|osDescription|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|ownerType|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|inGracePeriodUntilDateTime|DateTimeOffset|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedDeviceCompliance](../resources/manageddevicecompliance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_manageddevicecompliance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/managedDeviceCompliances/{managedDeviceCompliancesId}
Content-Type: application/json
Content-length: 545

{
  "@odata.type": "#microsoft.graph.managedDeviceCompliance",
  "organizationId": "String",
  "organizationDisplayName": "String",
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
  "@odata.type": "#microsoft.graph.managedDeviceCompliance",
  "id": "25b3eecc-eecc-25b3-ccee-b325cceeb325",
  "organizationId": "String",
  "organizationDisplayName": "String",
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

