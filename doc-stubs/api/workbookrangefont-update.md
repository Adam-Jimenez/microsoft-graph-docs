---
title: "Update workbookRangeFont"
description: "Update the properties of a workbookRangeFont object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update workbookRangeFont
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [workbookRangeFont](../resources/workbookrangefont.md) object.

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
PATCH /workbookRange/format/font
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeFont](../resources/workbookrangefont.md) object.

The following table shows the properties that are required when you update the [workbookRangeFont](../resources/workbookrangefont.md).

|Property|Type|Description|
|:---|:---|:---|
|bold|Boolean|**TODO: Add Description**|
|color|String|**TODO: Add Description**|
|italic|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|size|Double|**TODO: Add Description**|
|underline|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookrangefont"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbookRange/format/font
Content-Type: application/json
Content-length: 195

{
  "@odata.type": "#microsoft.graph.workbookRangeFont",
  "bold": "Boolean",
  "color": "String",
  "italic": "Boolean",
  "name": "String",
  "size": "Double",
  "underline": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.workbookRangeFont",
  "bold": "Boolean",
  "color": "String",
  "italic": "Boolean",
  "name": "String",
  "size": "Double",
  "underline": "String"
}
```

