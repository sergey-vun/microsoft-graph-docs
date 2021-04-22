---
title: "Create managedTenantAdditionalInfo"
description: "Create a new managedTenantAdditionalInfo object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedTenantAdditionalInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object.

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
POST /managedTenantAdditionalInfo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object.

The following table shows the properties that are required when you create the [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|contactInfo|[ContactInfo](../resources/contactinfo.md) collection|**TODO: Add Description**|
|partnerId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedTenantAdditionalInfo](../resources/managedtenantadditionalinfo.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedtenantadditionalinfo_from_managedtenantadditionalinfo"
}
-->
``` http
POST https://graph.microsoft.com/beta/managedTenantAdditionalInfo
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.management.services.api.managedTenantAdditionalInfo",
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
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedTenantAdditionalInfo"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.managedTenantAdditionalInfo",
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

