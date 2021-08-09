---
title: "Create workbookRangeView"
description: "Create a new workbookRangeView object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookRangeView
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [workbookRangeView](../resources/workbookrangeview.md) object.

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
POST /workbookRangeView/rows
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeView](../resources/workbookrangeview.md) object.

The following table shows the properties that are required when you create the [workbookRangeView](../resources/workbookrangeview.md).

|Property|Type|Description|
|:---|:---|:---|
|cellAddresses|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|columnCount|Int32|**TODO: Add Description**|
|formulas|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|formulasLocal|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|formulasR1C1|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|index|Int32|**TODO: Add Description**|
|numberFormat|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|rowCount|Int32|**TODO: Add Description**|
|text|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|valueTypes|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|
|values|[Microsoft.ExcelServices.Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookRangeView](../resources/workbookrangeview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookrangeview_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbookRangeView/rows
Content-Type: application/json
Content-length: 687

{
  "@odata.type": "#Microsoft.ExcelServices.workbookRangeView",
  "cellAddresses": {
    "@odata.type": "microsoft.graph.Json"
  },
  "columnCount": "Integer",
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "index": "Integer",
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": "Integer",
  "text": {
    "@odata.type": "microsoft.graph.Json"
  },
  "valueTypes": {
    "@odata.type": "microsoft.graph.Json"
  },
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
  "@odata.type": "Microsoft.ExcelServices.workbookRangeView"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.ExcelServices.workbookRangeView",
  "cellAddresses": {
    "@odata.type": "microsoft.graph.Json"
  },
  "columnCount": "Integer",
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "index": "Integer",
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": "Integer",
  "text": {
    "@odata.type": "microsoft.graph.Json"
  },
  "valueTypes": {
    "@odata.type": "microsoft.graph.Json"
  },
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

