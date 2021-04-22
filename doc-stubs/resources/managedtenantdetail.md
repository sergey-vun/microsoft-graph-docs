---
title: "managedTenantDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedTenantDetail resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedTenantDetails](../api/managedtenantdetail-list.md)|[managedTenantDetail](../resources/managedtenantdetail.md) collection|Get a list of the [managedTenantDetail](../resources/managedtenantdetail.md) objects and their properties.|
|[Create managedTenantDetail](../api/managedtenantdetail-post-managedtenantdetails.md)|[managedTenantDetail](../resources/managedtenantdetail.md)|Create a new [managedTenantDetail](../resources/managedtenantdetail.md) object.|
|[Get managedTenantDetail](../api/managedtenantdetail-get.md)|[managedTenantDetail](../resources/managedtenantdetail.md)|Read the properties and relationships of a [managedTenantDetail](../resources/managedtenantdetail.md) object.|
|[Update managedTenantDetail](../api/managedtenantdetail-update.md)|[managedTenantDetail](../resources/managedtenantdetail.md)|Update the properties of a [managedTenantDetail](../resources/managedtenantdetail.md) object.|
|[Delete managedTenantDetail](../api/managedtenantdetail-delete.md)|None|Deletes a [managedTenantDetail](../resources/managedtenantdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|countryCode|String|**TODO: Add Description**|
|countryName|String|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|industryName|String|**TODO: Add Description**|
|organizationId|String|**TODO: Add Description**|
|region|String|**TODO: Add Description**|
|segmentName|String|**TODO: Add Description**|
|subSegmentName|String|**TODO: Add Description**|
|verticalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenantDetail",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenantDetail",
  "organizationId": "String",
  "companyName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String",
  "subSegmentName": "String"
}
```

