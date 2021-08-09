---
title: "Create workbookFormatProtection"
description: "Create a new workbookFormatProtection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookFormatProtection
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [workbookFormatProtection](../resources/workbookformatprotection.md) object.

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
POST ** Collection URI for Microsoft.ExcelServices.workbookFormatProtection not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookFormatProtection](../resources/workbookformatprotection.md) object.

The following table shows the properties that are required when you create the [workbookFormatProtection](../resources/workbookformatprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|formulaHidden|Boolean|**TODO: Add Description**|
|locked|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookFormatProtection](../resources/workbookformatprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookformatprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for Microsoft.ExcelServices.workbookFormatProtection not found
Content-Type: application/json
Content-length: 129

{
  "@odata.type": "#Microsoft.ExcelServices.workbookFormatProtection",
  "formulaHidden": "Boolean",
  "locked": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookFormatProtection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookFormatProtection",
  "formulaHidden": "Boolean",
  "locked": "Boolean"
}
```

