---
title: "List restrictedSignIns"
description: "Get the restrictedSignIn resources from the restrictedSignIns navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List restrictedSignIns
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the restrictedSignIn resources from the restrictedSignIns navigation property.

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
GET /auditLogs/restrictedSignIns
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [restrictedSignIn](../resources/restrictedsignin.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.restrictedSignIn)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedSignIn",
      "id": "96650862-0862-9665-6208-659662086596",
      "alternateSignInName": "String",
      "appDisplayName": "String",
      "appId": "String",
      "appliedConditionalAccessPolicies": [
        {
          "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
        }
      ],
      "authenticationDetails": [
        {
          "@odata.type": "microsoft.graph.authenticationDetail"
        }
      ],
      "authenticationMethodsUsed": [
        "String"
      ],
      "authenticationProcessingDetails": [
        {
          "@odata.type": "microsoft.graph.keyValue"
        }
      ],
      "authenticationRequirement": "String",
      "authenticationRequirementPolicies": [
        {
          "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
        }
      ],
      "clientAppUsed": "String",
      "conditionalAccessStatus": "String",
      "correlationId": "String",
      "createdDateTime": "String (timestamp)",
      "deviceDetail": {
        "@odata.type": "microsoft.graph.deviceDetail"
      },
      "flaggedForReview": "Boolean",
      "homeTenantId": "String",
      "isInteractive": "Boolean",
      "ipAddress": "String",
      "ipAddressFromResourceProvider": "String",
      "location": {
        "@odata.type": "microsoft.graph.signInLocation"
      },
      "mfaDetail": {
        "@odata.type": "microsoft.graph.mfaDetail"
      },
      "networkLocationDetails": [
        {
          "@odata.type": "microsoft.graph.networkLocationDetail"
        }
      ],
      "originalRequestId": "String",
      "processingTimeInMilliseconds": "Integer",
      "riskDetail": "String",
      "riskEventTypes": [
        "String"
      ],
      "riskEventTypes_v2": [
        "String"
      ],
      "riskLevelAggregated": "String",
      "riskLevelDuringSignIn": "String",
      "riskState": "String",
      "resourceDisplayName": "String",
      "resourceId": "String",
      "resourceTenantId": "String",
      "servicePrincipalId": "String",
      "servicePrincipalName": "String",
      "signInEventTypes": [
        "String"
      ],
      "signInIdentifier": "String",
      "signInIdentifierType": "String",
      "status": {
        "@odata.type": "microsoft.graph.signInStatus"
      },
      "tokenIssuerName": "String",
      "tokenIssuerType": "String",
      "userAgent": "String",
      "userDisplayName": "String",
      "userId": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "targetTenantId": "Guid"
    }
  ]
}
```

