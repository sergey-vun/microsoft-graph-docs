---
title: "Update managedTenantAdditionalInfo"
description: "Update the properties of a managedTenantAdditionalInfo object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedTenantAdditionalInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object.

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
PATCH /managedTenantAdditionalInfo/{managedTenantAdditionalInfoId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object.

The following table shows the properties that are required when you update the [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|contactInfo|[ContactInfo](../resources/contactinfo.md) collection|**TODO: Add Description**|
|partnerId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedtenantadditionalinfo"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/managedTenantAdditionalInfo/{managedTenantAdditionalInfoId}
Content-Type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.managedTenantAdditionalInfo",
  "contactInfo": [
    {
      "@odata.type": "microsoft.graph.ContactInfo"
    }
  ],
  "partnerId": "String",
  "azureTenantId": "String",
  "website": "String",
  "etag": "String"
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
  "@odata.type": "#microsoft.graph.managedTenantAdditionalInfo",
  "id": "ebea4a29-4a29-ebea-294a-eaeb294aeaeb",
  "contactInfo": [
    {
      "@odata.type": "microsoft.graph.ContactInfo"
    }
  ],
  "partnerId": "String",
  "azureTenantId": "String",
  "website": "String",
  "etag": "String"
}
```

