---
title: "managementTemplateStepDeployment: changeDeploymentStatus"
description: "Changes the status for the management template step."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: apiPageType
---

# managementTemplateStepDeployment: changeDeploymentStatus
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Changes the status for the [management template step](../resources/managedtenants-managementtemplatestep.md). This information is used to provide insights into what management actions are in a specific state. As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ManagedTenants.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementTemplateStepDeployments/changeDeploymentStatus?$expand=templateStepVersion
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
|tenantId|String|The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).|
|managementTemplateStepId|String|The identifier for the management template step.|
|status|String|The updated status for the [management template step](../resources/managedtenants-managementtemplatestep.md). Possible values include: `toAddress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, and `riskAccepted`.|

## Response

If successful, this action returns a `200 OK` response code and a [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "managementtemplatestepdeploymentthis.changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplateStepDeployments/changeDeploymentStatus?$expand=templateStepVersion
Content-Type: application/json
Content-length: 92

{
  "tenantId": "15b5e82f-b10d-4709-81b6-c74660993a35",
  "managementTemplateStepId": "12524106-036f-457f-b7a6-b003509d29c8_1",
  "status": "toAddress"
}
```

### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepDeployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "tenantId": "15b5e82f-b10d-4709-81b6-c74660993a35",
  "templateStepVersion": {
    "id": "12524106-036f-457f-b7a6-b003509d29c8_1",
    "version": 1,
    "configurationAction": {
      "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
      "category": "automated",
      "licenses": {
        "servicePlans": [
          {
            "appliesTo": "67866ca8-edf3-4155-aef2-05d2b932bae4",
            "provisioningStatus": "Provisioned",
            "servicePlanId": "ebb9db73-6053-4cec-bad0-a0ca7250e5cc",
            "servicePlanName": "AAD_PREMIUM"
          }
        ],
        "skuId": "b7d22525-bfb1-4804-b3ca-c076ca36c0d0",
        "skuPartNumber": "cc6ed3af-1fe5-40c4-b9ca-d489875d28f4"
      },
      "displayName": "ConditionalAccessPolicy",
      "description": null,
      "service": null,
      "settings": [
        {
          "settingId": "d7f40dd7-5a73-43a8-bb58-ee86ca3c58cf",
          "valueType": "string",
          "displayName": "DisplayName",
          "overwriteAllowed": false,
          "jsonValue": "\"Baseline – Require MFA for Admins\""
        },
        {
          "settingId": "463f6c99-a6ae-4e14-9c3e-f6cf86f25002",
          "valueType": "string",
          "displayName": "State",
          "overwriteAllowed": false,
          "jsonValue": "\"enabledForReportingButNotEnforced\""
        },
        {
          "settingId": "0fc34283-497d-43a0-a057-99be38a0ac5f",
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "f79d4264-0a3a-4de5-830c-8bde23c8e43c",
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "faacbde9-ae4f-4b47-af0a-ae534b72ab61",
          "valueType": "stringCollection",
          "displayName": "IncludeRoles",
          "overwriteAllowed": false,
          "jsonValue": "[\"62e90394-69f5-4237-9190-012177145e10\",\"f28a1f50-f6e7-4571-818b-6a12f2af6b6c\",\"29232cdf-9323-42fd-ade2-1d097af3e4de\",\"b1be1c3e-b65d-4f19-8427-f6fa0d97feb9\",\"194ae4cb-b126-40b2-bd5b-6091b380977d\",\"729827e3-9c14-49f7-bb1b-9608f156bbb8\",\"b0f54661-2d74-4c50-afa3-1ec803f12efe\",\"fe930be7-5e62-47db-91af-98c3a49a38b1\",\"c4e39bd9-1100-46d3-8c65-fb160da0071f\"]"
        },
        {
          "settingId": "806e61d5-3c22-4784-94bb-58fe32fed473",
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "deff85c4-74e1-46f0-b69d-f5b124f0f1cb",
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "overwriteAllowed": false,
          "jsonValue": "\"OR\""
        },
        {
          "settingId": "deff85c4-74e1-46f0-b69d-f5b124f0f1cb",
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "overwriteAllowed": false,
          "jsonValue": "[\"mfa\"]"
        }
      ],
      "operationDefinition": {
        "values": [
          "POST /beta/groups/[@sys.project([/beta/groups?$filter=displayName eq 'MFA'],\"id\")]/members/$ref\\ { \"@odata.id\": \"https://graph.microsoft.com/beta/directoryObjects/[@sys.project([/beta/users?$filter=createdDateTime le 2021-01-01T00:00:00Z&$top=500],\"id\")]\" }"
        ],
        "failOnError": true,
        "managedTenantOperationLogLevel": "full"
      },
      "aggregationDefinition": {
        "values": [ "@sys.append([/result])" ],
        "failOnError": true,
        "managedTenantOperationLogLevel": "full"
      }
    }
  },
  "status": "toAddress"
}
```
