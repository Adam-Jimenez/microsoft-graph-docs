---
title: "workbookNamedItem: add"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# workbookNamedItem: add
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
POST /driveItem/workbook/names/add
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
|name|String|**TODO: Add Description**|
|reference|[Json](../resources/json.md)|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [workbookNamedItem](../resources/workbooknameditem.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbooknameditem_add"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/add
Content-Type: application/json
Content-length: 115

{
  "name": "String",
  "reference": {
    "@odata.type": "microsoft.graph.Json"
  },
  "comment": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookNamedItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.ExcelServices.workbookNamedItem",
    "comment": "String",
    "name": "String",
    "scope": "String",
    "type": "String",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    },
    "visible": "Boolean",
    "_Id": "String"
  }
}
```

