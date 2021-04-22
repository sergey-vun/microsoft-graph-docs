---
title: "Update deviceCompliancePolicySettingStateSummary"
description: "Update the properties of a deviceCompliancePolicySettingStateSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceCompliancePolicySettingStateSummary
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.

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
PATCH /deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummariesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.

The following table shows the properties that are required when you update the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|intuneAccountId|String|**TODO: Add Description**|
|intuneSettingId|String|**TODO: Add Description**|
|policyType|String|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|pendingDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|succeededDeviceCount|Int32|**TODO: Add Description**|
|failedDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancepolicysettingstatesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummariesId}
Content-Type: application/json
Content-length: 545

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "organizationId": "String",
  "organizationDisplayName": "String",
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
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "c9a0db79-db79-c9a0-79db-a0c979dba0c9",
  "organizationId": "String",
  "organizationDisplayName": "String",
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

