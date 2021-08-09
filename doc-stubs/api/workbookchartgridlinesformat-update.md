---
title: "Update workbookChartGridlinesFormat"
description: "Update the properties of a workbookChartGridlinesFormat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update workbookChartGridlinesFormat
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.

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
PATCH /driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/majorGridlines/format
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.

The following table shows the properties that are required when you update the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md).

|Property|Type|Description|
|:---|:---|:---|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookchartgridlinesformat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/majorGridlines/format
Content-Type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.workbookChartGridlinesFormat"
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
  "@odata.type": "#microsoft.graph.workbookChartGridlinesFormat"
}
```

