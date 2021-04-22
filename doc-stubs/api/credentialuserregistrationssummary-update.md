---
title: "Update credentialUserRegistrationsSummary"
description: "Update the properties of a credentialUserRegistrationsSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update credentialUserRegistrationsSummary
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) object.

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
PATCH /credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummariesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) object.

The following table shows the properties that are required when you update the [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|mfaAndSsprCapableUserCount|Int32|**TODO: Add Description**|
|ssprEnabledUserCount|Int32|**TODO: Add Description**|
|mfaRegisteredUserCount|Int32|**TODO: Add Description**|
|ssprRegisteredUserCount|Int32|**TODO: Add Description**|
|totalUserCount|Int32|**TODO: Add Description**|
|securityDefaultsEnabled|Boolean|**TODO: Add Description**|
|mfaConditionalAccessPolicyState|String|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_credentialuserregistrationssummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummariesId}
Content-Type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationsSummary",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
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
  "@odata.type": "#microsoft.graph.credentialUserRegistrationsSummary",
  "id": "6f76b50b-b50b-6f76-0bb5-766f0bb5766f",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

