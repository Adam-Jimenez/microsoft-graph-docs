---
title: "workbookTable: dataBodyRange"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# workbookTable: dataBodyRange
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
GET /driveItem/workbook/tables/{workbookTableId}/dataBodyRange
GET /driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/dataBodyRange
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [workbookRange](../resources/workbookrange.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbooktable_databodyrange"
}
-->
``` http
GET https://graph.microsoft.com/beta/driveItem/workbook/tables/{workbookTableId}/dataBodyRange
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookRange"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.ExcelServices.workbookRange",
    "address": "String",
    "addressLocal": "String",
    "cellCount": "Integer",
    "columnCount": "Integer",
    "columnHidden": "Boolean",
    "columnIndex": "Integer",
    "formulas": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasLocal": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasR1C1": {
      "@odata.type": "microsoft.graph.Json"
    },
    "hidden": "Boolean",
    "numberFormat": {
      "@odata.type": "microsoft.graph.Json"
    },
    "rowCount": "Integer",
    "rowHidden": "Boolean",
    "rowIndex": "Integer",
    "text": {
      "@odata.type": "microsoft.graph.Json"
    },
    "valueTypes": {
      "@odata.type": "microsoft.graph.Json"
    },
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

