---
title: "Create conditionalAccessPolicyCoverage"
description: "Create a new conditionalAccessPolicyCoverage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create conditionalAccessPolicyCoverage
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.

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
POST /conditionalAccessPolicyCoverages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object.

The following table shows the properties that are required when you create the [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|organizationDisplayName|String|**TODO: Add Description**|
|conditionalAccessPolicyState|String|**TODO: Add Description**|
|requiresDeviceCompliance|Boolean|**TODO: Add Description**|
|latestPolicyModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [conditionalAccessPolicyCoverage](../resources/conditionalaccesspolicycoverage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicycoverage_from_conditionalaccesspolicycoverages"
}
-->
``` http
POST https://graph.microsoft.com/beta/conditionalAccessPolicyCoverages
Content-Type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.management.services.api.conditionalAccessPolicyCoverage",
  "organizationDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.conditionalAccessPolicyCoverage",
  "id": "baa2983f-983f-baa2-3f98-a2ba3f98a2ba",
  "organizationDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```

