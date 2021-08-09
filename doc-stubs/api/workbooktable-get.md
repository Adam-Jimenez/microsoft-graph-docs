---
title: "Get workbookTable"
description: "Read the properties and relationships of a workbookTable object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get workbookTable
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [workbookTable](../resources/workbooktable.md) object.

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
GET /driveItem/workbook/tables/{workbookTableId}
GET /driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbooktable"
}
-->
``` http
GET https://graph.microsoft.com/beta/driveItem/workbook/tables/{workbookTableId}
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
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

