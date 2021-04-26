---
title: "credentialUserRegistrationsSummary resource type"
description: "Represents a summary of the number of users across managed tenants that have multi-factor authentication enabled."
author: "isaiahwilliams"
localization_priority: Normal
ms.prod: "microsoft365-lighthouse"
doc_type: resourcePageType
---

# credentialUserRegistrationsSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List credentialUserRegistrationsSummaries](../api/credentialuserregistrationssummary-list.md)|[credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) collection|Get a list of the [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) objects and their properties.|
|[Get credentialUserRegistrationsSummary](../api/credentialuserregistrationssummary-get.md)|[credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md)|Read the properties and relationships of a [credentialUserRegistrationsSummary](../resources/credentialuserregistrationssummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier for this entity.|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|mfaAndSsprCapableUserCount|Int32|**TODO: Add Description**|
|mfaConditionalAccessPolicyState|String|**TODO: Add Description**|
|mfaRegisteredUserCount|Int32|**TODO: Add Description**|
|securityDefaultsEnabled|Boolean|**TODO: Add Description**|
|ssprEnabledUserCount|Int32|**TODO: Add Description**|
|ssprRegisteredUserCount|Int32|**TODO: Add Description**|
|tenantDisplayName|String|Display name for the managed tenant.|
|tenantId|String|The unique identifier for the managed tenant.|
|totalUserCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.credentialUserRegistrationsSummary",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationsSummary",
  "id": "String (identifier)",
  "organizationId": "String",
  "organizationDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

