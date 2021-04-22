---
title: "Update Customer"
description: "Update the properties of a Customer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update Customer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [Customer](../resources/customer.md) object.

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
PATCH /Customers/{CustomersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [Customer](../resources/customer.md) object.

The following table shows the properties that are required when you update the [Customer](../resources/customer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|partnerId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|contractId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|domain|String|**TODO: Add Description**|
|contractType|Int32|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|isOnBoardedToMTM|Boolean|**TODO: Add Description**|
|onboardingStatus|Int32|**TODO: Add Description**|
|delegatedPrivilegeStatus|Int32|**TODO: Add Description**|
|lastDAPRefreshDateTimeUtc|DateTimeOffset|**TODO: Add Description**|
|cosmosCreatedDateTimeUTC|DateTimeOffset|**TODO: Add Description**|
|cosmosLastModifiedDateTimeUTC|DateTimeOffset|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [Customer](../resources/customer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_customer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Customers/{CustomersId}
Content-Type: application/json
Content-length: 594

{
  "@odata.type": "#microsoft.graph.Customer",
  "partnerId": "String",
  "azureTenantId": "String",
  "contractId": "String",
  "displayName": "String",
  "domain": "String",
  "contractType": "Integer",
  "countryLetterCode": "String",
  "deletedDateTime": "String (timestamp)",
  "isOnBoardedToMTM": "Boolean",
  "onboardingStatus": "Integer",
  "delegatedPrivilegeStatus": "Integer",
  "lastDAPRefreshDateTimeUtc": "String (timestamp)",
  "cosmosCreatedDateTimeUTC": "String (timestamp)",
  "cosmosLastModifiedDateTimeUTC": "String (timestamp)",
  "isDeleted": "Boolean"
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
  "@odata.type": "#microsoft.graph.Customer",
  "id": "52dde42a-e42a-52dd-2ae4-dd522ae4dd52",
  "partnerId": "String",
  "azureTenantId": "String",
  "contractId": "String",
  "displayName": "String",
  "domain": "String",
  "contractType": "Integer",
  "countryLetterCode": "String",
  "deletedDateTime": "String (timestamp)",
  "isOnBoardedToMTM": "Boolean",
  "onboardingStatus": "Integer",
  "delegatedPrivilegeStatus": "Integer",
  "lastDAPRefreshDateTimeUtc": "String (timestamp)",
  "cosmosCreatedDateTimeUTC": "String (timestamp)",
  "cosmosLastModifiedDateTimeUTC": "String (timestamp)",
  "isDeleted": "Boolean"
}
```

