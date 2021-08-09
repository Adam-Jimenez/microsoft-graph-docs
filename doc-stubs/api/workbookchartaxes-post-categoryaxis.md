---
title: "Create workbookChartAxis"
description: "Create a new workbookChartAxis object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookChartAxis
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookChartAxis object.

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
POST /driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartAxis](../resources/workbookchartaxis.md) object.

The following table shows the properties that are required when you create the [workbookChartAxis](../resources/workbookchartaxis.md).

|Property|Type|Description|
|:---|:---|:---|
|majorUnit|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|maximum|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|minimum|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|minorUnit|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookChartAxis](../resources/workbookchartaxis.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookchartaxis_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis
Content-Type: application/json
Content-length: 331

{
  "@odata.type": "#Microsoft.ExcelServices.workbookChartAxis",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookChartAxis"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookChartAxis",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

