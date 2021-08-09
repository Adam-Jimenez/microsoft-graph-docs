---
title: "Update workbookCommentReply"
description: "Update the properties of a workbookCommentReply object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update workbookCommentReply
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [workbookCommentReply](../resources/workbookcommentreply.md) object.

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
PATCH /driveItem/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookCommentReply](../resources/workbookcommentreply.md) object.

The following table shows the properties that are required when you update the [workbookCommentReply](../resources/workbookcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookcommentreply"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/driveItem/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
Content-Type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "content": "String",
  "contentType": "String"
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
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "content": "String",
  "contentType": "String",
  "id": "05c24a5e-4a5e-05c2-5e4a-c2055e4ac205"
}
```

