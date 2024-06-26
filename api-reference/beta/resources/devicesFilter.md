---
title: "devicesFilter resource type"
description: Defines the the rule to filter the devices and whether devices satisfying the rule should be allowed or blocked. **devicesFilter is not yet implemented.**
author: "vimrang"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# devicesFilter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Not implemented yet**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|mode|crossTenantAccessPolicyTargetConfigurationAccessType|Determines whether devices satisfying the rule should be allowed or blocked.The possible values are: `allowed`, `blocked`, `unknownFutureValue`.**Not implemented yet**|
|rule|String|Defines the rule to filter the devices. An example would be `device.deviceAttribute2 -eq 'PrivilegedAccessWorkstation'` **Not implemented yet**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.devicesFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.devicesFilter",
  "mode": "String",
  "rule": "String"
}
```