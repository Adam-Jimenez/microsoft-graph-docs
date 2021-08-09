---
title: "workbookWorksheetProtection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookWorksheetProtection resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List workbookWorksheetProtections](../api/workbookworksheetprotection-list.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md) collection|Get a list of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects and their properties.|
|[Create workbookWorksheetProtection](../api/workbookworksheetprotection-create.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Create a new [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Get workbookWorksheetProtection](../api/workbookworksheetprotection-get.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Read the properties and relationships of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Update workbookWorksheetProtection](../api/workbookworksheetprotection-update.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Update the properties of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Delete workbookWorksheetProtection](../api/workbookworksheetprotection-delete.md)|None|Deletes a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[protect](../api/workbookworksheetprotection-protect.md)|None|**TODO: Add Description**|
|[unprotect](../api/workbookworksheetprotection-unprotect.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|options|[workbookWorksheetProtectionOptions](../resources/workbookworksheetprotectionoptions.md)|**TODO: Add Description**|
|protected|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
  },
  "protected": "Boolean"
}
```

