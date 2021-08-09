---
title: "Create workbookTableSort"
description: "Create a new workbookTableSort object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookTableSort
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookTableSort object.

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
POST /driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookTableSort](../resources/workbooktablesort.md) object.

The following table shows the properties that are required when you create the [workbookTableSort](../resources/workbooktablesort.md).

|Property|Type|Description|
|:---|:---|:---|
|fields|[Microsoft.ExcelServices.workbookSortField](../resources/workbooksortfield.md) collection|**TODO: Add Description**|
|matchCase|Boolean|**TODO: Add Description**|
|method|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookTableSort](../resources/workbooktablesort.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktablesort_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
Content-Type: application/json
Content-length: 210

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTableSort",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField"
    }
  ],
  "matchCase": "Boolean",
  "method": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookTableSort"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookTableSort",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField"
    }
  ],
  "matchCase": "Boolean",
  "method": "String"
}
```

