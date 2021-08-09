---
title: "Create workbookChart"
description: "Create a new workbookChart object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookChart
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookChart object.

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
POST /driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChart](../resources/workbookchart.md) object.

The following table shows the properties that are required when you create the [workbookChart](../resources/workbookchart.md).

|Property|Type|Description|
|:---|:---|:---|
|height|Double|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|left|Double|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|top|Double|**TODO: Add Description**|
|width|Double|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookChart](../resources/workbookchart.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookchart_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#Microsoft.ExcelServices.workbookChart",
  "height": "Double",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookChart"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookChart",
  "height": "Double",
  "id": "4d92798b-798b-4d92-8b79-924d8b79924d",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
}
```

