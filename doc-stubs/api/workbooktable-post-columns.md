---
title: "Create workbookTableColumn"
description: "Create a new workbookTableColumn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookTableColumn
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookTableColumn object.

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
POST /driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookTableColumn](../resources/workbooktablecolumn.md) object.

The following table shows the properties that are required when you create the [workbookTableColumn](../resources/workbooktablecolumn.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|index|Int32|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|values|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktablecolumn_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
Content-Type: application/json
Content-length: 177

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTableColumn",
  "index": "Integer",
  "name": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTableColumn",
  "id": "4223f2e4-f2e4-4223-e4f2-2342e4f22342",
  "index": "Integer",
  "name": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

