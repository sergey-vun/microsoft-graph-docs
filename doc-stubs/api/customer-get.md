---
title: "Get Customer"
description: "Read the properties and relationships of a Customer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get Customer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [Customer](../resources/customer.md) object.

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
GET /Customers/{CustomersId}
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

If successful, this method returns a `200 OK` response code and a [Customer](../resources/customer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/beta/Customers/{CustomersId}
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
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

