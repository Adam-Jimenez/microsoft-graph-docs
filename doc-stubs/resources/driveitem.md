---
title: "driveItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# driveItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List driveItems](../api/driveitem-list.md)|[driveItem](../resources/driveitem.md) collection|Get a list of the [driveItem](../resources/driveitem.md) objects and their properties.|
|[Create driveItem](../api/driveitem-create.md)|[driveItem](../resources/driveitem.md)|Create a new [driveItem](../resources/driveitem.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[Update driveItem](../api/driveitem-update.md)|[driveItem](../resources/driveitem.md)|Update the properties of a [driveItem](../resources/driveitem.md) object.|
|[Delete driveItem](../api/driveitem-delete.md)|None|Deletes a [driveItem](../resources/driveitem.md) object.|
|[List workbook](../api/driveitem-list-workbook.md)|[workbook](../resources/workbook.md) collection|Get the workbook resources from the workbook navigation property.|
|[Create workbook](../api/driveitem-post-workbook.md)|[workbook](../resources/workbook.md)|Create a new workbook object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|workbook|[workbook](../resources/workbook.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItem"
}
```

