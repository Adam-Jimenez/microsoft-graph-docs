---
title: "Update workbookRangeFormat"
description: "Update the properties of a workbookRangeFormat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update workbookRangeFormat
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [workbookRangeFormat](../resources/workbookrangeformat.md) object.

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
PATCH /workbookRange/format
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.

The following table shows the properties that are required when you update the [workbookRangeFormat](../resources/workbookrangeformat.md).

|Property|Type|Description|
|:---|:---|:---|
|columnWidth|Double|**TODO: Add Description**|
|horizontalAlignment|String|**TODO: Add Description**|
|rowHeight|Double|**TODO: Add Description**|
|verticalAlignment|String|**TODO: Add Description**|
|wrapText|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookrangeformat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbookRange/format
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "columnWidth": "Double",
  "horizontalAlignment": "String",
  "rowHeight": "Double",
  "verticalAlignment": "String",
  "wrapText": "Boolean"
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
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "columnWidth": "Double",
  "horizontalAlignment": "String",
  "rowHeight": "Double",
  "verticalAlignment": "String",
  "wrapText": "Boolean"
}
```

