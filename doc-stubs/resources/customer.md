---
title: "Customer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# Customer resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List Customers](../api/customer-list.md)|[Customer](../resources/customer.md) collection|Get a list of the [Customer](../resources/customer.md) objects and their properties.|
|[Create Customer](../api/customer-post-customers.md)|[Customer](../resources/customer.md)|Create a new [Customer](../resources/customer.md) object.|
|[Get Customer](../api/customer-get.md)|[Customer](../resources/customer.md)|Read the properties and relationships of a [Customer](../resources/customer.md) object.|
|[Update Customer](../api/customer-update.md)|[Customer](../resources/customer.md)|Update the properties of a [Customer](../resources/customer.md) object.|
|[Delete Customer](../api/customer-delete.md)|None|Deletes a [Customer](../resources/customer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureTenantId|String|**TODO: Add Description**|
|contractId|String|**TODO: Add Description**|
|contractType|Int32|**TODO: Add Description**|
|cosmosCreatedDateTimeUTC|DateTimeOffset|**TODO: Add Description**|
|cosmosLastModifiedDateTimeUTC|DateTimeOffset|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|delegatedPrivilegeStatus|Int32|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|domain|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|
|isOnBoardedToMTM|Boolean|**TODO: Add Description**|
|lastDAPRefreshDateTimeUtc|DateTimeOffset|**TODO: Add Description**|
|onboardingStatus|Int32|**TODO: Add Description**|
|partnerId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.Customer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Customer",
  "id": "String (identifier)",
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

