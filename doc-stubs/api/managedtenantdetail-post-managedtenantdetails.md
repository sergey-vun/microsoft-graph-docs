---
title: "Create managedTenantDetail"
description: "Create a new managedTenantDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedTenantDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [managedTenantDetail](../resources/managedtenantdetail.md) object.

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
POST /managedTenantDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantDetail](../resources/managedtenantdetail.md) object.

The following table shows the properties that are required when you create the [managedTenantDetail](../resources/managedtenantdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|organizationId|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|countryName|String|**TODO: Add Description**|
|countryCode|String|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|region|String|**TODO: Add Description**|
|verticalName|String|**TODO: Add Description**|
|industryName|String|**TODO: Add Description**|
|segmentName|String|**TODO: Add Description**|
|subSegmentName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedTenantDetail](../resources/managedtenantdetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedtenantdetail_from_managedtenantdetails"
}
-->
``` http
POST https://graph.microsoft.com/beta/managedTenantDetails
Content-Type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.management.services.api.managedTenantDetail",
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


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedTenantDetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.managedTenantDetail",
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

