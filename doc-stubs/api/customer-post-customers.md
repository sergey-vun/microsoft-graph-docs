---
title: "Create Customer"
description: "Create a new Customer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create Customer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [Customer](../resources/customer.md) object.

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
POST /Customers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [Customer](../resources/customer.md) object.

The following table shows the properties that are required when you create the [Customer](../resources/customer.md).

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

If successful, this method returns a `201 Created` response code and a [Customer](../resources/customer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_customer_from_customers"
}
-->
``` http
POST https://graph.microsoft.com/beta/Customers
Content-Type: application/json
Content-length: 612

{
  "@odata.type": "#microsoft.management.services.api.Customer",
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
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.Customer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.Customer",
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

