---
title: "workbookFunctions: quartile_Inc"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# workbookFunctions: quartile_Inc
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
POST /driveItem/workbook/functions/quartile_Inc
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
|array|[Json](../resources/json.md)|**TODO: Add Description**|
|quart|[Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_quartile_inc"
}
-->
``` http
POST https://graph.microsoft.com/beta/driveItem/workbook/functions/quartile_Inc
Content-Type: application/json
Content-length: 129

{
  "array": {
    "@odata.type": "microsoft.graph.Json"
  },
  "quart": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.ExcelServices.workbookFunctionResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.ExcelServices.workbookFunctionResult",
    "error": "String",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

