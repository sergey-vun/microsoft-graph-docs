---
title: "Create cloudPcDevice"
description: "Create a new cloudPcDevice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cloudPcDevice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [cloudPcDevice](../resources/cloudpcdevice.md) object.

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
POST /cloudPcDevices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcDevice](../resources/cloudpcdevice.md) object.

The following table shows the properties that are required when you create the [cloudPcDevice](../resources/cloudpcdevice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|servicePlanName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|lastUpdated|DateTimeOffset|**TODO: Add Description**|
|policyId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [cloudPcDevice](../resources/cloudpcdevice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_cloudpcdevice_from_cloudpcdevices"
}
-->
``` http
POST https://graph.microsoft.com/beta/cloudPcDevices
Content-Type: application/json
Content-length: 392

{
  "@odata.type": "#microsoft.management.services.api.cloudPcDevice",
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


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.cloudPcDevice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.cloudPcDevice",
  "id": "89cbd202-d202-89cb-02d2-cb8902d2cb89",
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

