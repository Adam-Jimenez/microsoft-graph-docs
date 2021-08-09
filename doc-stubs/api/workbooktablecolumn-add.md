---
title: "workbookTableColumn: add"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# workbookTableColumn: add
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
POST /driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/add
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|index|Int32|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [workbookTableColumn](../resources/workbooktablecolumn.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbooktablecolumn_add"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/add
Content-Type: application/json
Content-length: 111

{
  "index": "Integer",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  },
  "name": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookTableColumn"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.ExcelServices.workbookTableColumn",
    "id": "String (identifier)",
    "index": "Integer",
    "name": "String",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

