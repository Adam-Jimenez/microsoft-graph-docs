---
title: "Create workbookTable"
description: "Create a new workbookTable object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookTable
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [workbookTable](../resources/workbooktable.md) object.

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
POST /driveItem/workbook/tables
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookTable](../resources/workbooktable.md) object.

The following table shows the properties that are required when you create the [workbookTable](../resources/workbooktable.md).

|Property|Type|Description|
|:---|:---|:---|
|highlightFirstColumn|Boolean|**TODO: Add Description**|
|highlightLastColumn|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|legacyId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|showBandedColumns|Boolean|**TODO: Add Description**|
|showBandedRows|Boolean|**TODO: Add Description**|
|showFilterButton|Boolean|**TODO: Add Description**|
|showHeaders|Boolean|**TODO: Add Description**|
|showTotals|Boolean|**TODO: Add Description**|
|style|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktable_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/tables
Content-Type: application/json
Content-length: 364

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTable",
  "highlightFirstColumn": "Boolean",
  "highlightLastColumn": "Boolean",
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": "Boolean",
  "showBandedRows": "Boolean",
  "showFilterButton": "Boolean",
  "showHeaders": "Boolean",
  "showTotals": "Boolean",
  "style": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookTable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTable",
  "highlightFirstColumn": "Boolean",
  "highlightLastColumn": "Boolean",
  "id": "43c4360e-360e-43c4-0e36-c4430e36c443",
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": "Boolean",
  "showBandedRows": "Boolean",
  "showFilterButton": "Boolean",
  "showHeaders": "Boolean",
  "showTotals": "Boolean",
  "style": "String"
}
```

