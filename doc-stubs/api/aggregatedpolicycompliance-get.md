---
title: "Get aggregatedPolicyCompliance"
description: "Read the properties and relationships of an aggregatedPolicyCompliance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get aggregatedPolicyCompliance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) object.

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
GET /aggregatedPolicyCompliances/{aggregatedPolicyCompliancesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/aggregatedPolicyCompliances/{aggregatedPolicyCompliancesId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.aggregatedPolicyCompliance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.management.services.api.aggregatedPolicyCompliance",
    "id": "06fcb4ea-b4ea-06fc-eab4-fc06eab4fc06",
    "organizationId": "String",
    "organizationDisplayName": "String",
    "compliancePolicyId": "String",
    "compliancePolicyName": "String",
    "compliancePolicyType": "String",
    "compliancePolicyPlatform": "String",
    "numberOfCompliantDevices": "Integer",
    "numberOfNonCompliantDevices": "Integer",
    "numberOfErrorDevices": "Integer",
    "policyModifiedDateTime": "String (timestamp)",
    "lastRefreshedDateTime": "String (timestamp)"
  }
}
```

