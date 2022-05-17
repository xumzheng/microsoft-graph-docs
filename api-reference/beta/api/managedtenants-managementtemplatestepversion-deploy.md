---
title: "managementTemplateStepVersion: deploy"
description: "Deploy the management template step version to the tenant where the configurations will be made."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: apiPageType
---

# managementTemplateStepVersion: deploy
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Deploy the [management template step version](../resources/managedtenants-managementtemplatestepversion.md) to the tenant where the configurations will be made.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementTemplateStepVersions/{managementTemplateStepVersionId}/deploy
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
|settingsList|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|The collection of settings to deploy.|

## Response

If successful, this action returns a `200 OK` response code and a [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "managementtemplatestepversionthis.deploy"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplateStepVersions/{managementTemplateStepVersionId}/deploy
Content-Type: application/json
Content-length: 132

{
  "tenantId": "6b0e46f8-4e82-4e58-8c0e-c9fe934c011d",
  "settingsList": [
    {
      "settingId": "65a48c58-b892-4d49-9450-ac20cb012e40",
      "valueType": "string",
      "displayName": "DisplayName",
      "overwriteAllowed": false,
      "jsonValue": "\"Baseline – Require MFA for Admins\""
    },
    {
      "settingId": "ca274d76-2426-4464-b5cb-34c3786f9b05",
      "valueType": "string",
      "displayName": "State",
      "overwriteAllowed": false,
      "jsonValue": "\"enabledForReportingButNotEnforced\""
    }
  ]
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
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#managementTemplateStepDeployment",
  "templateStepVersion": {
    "id": "b2d6d189-ea31-4cf8-b75e-41210c583127",
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
          "settingId": "5901d44a-b56b-4ae7-8bba-f767ccfc4539",
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "7c45112b-e82d-49ca-89f9-c448a7287dfa",
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "76cab0cf-f34a-4e66-8272-f5581dbdc0ac",
          "valueType": "stringCollection",
          "displayName": "IncludeRoles",
          "overwriteAllowed": false,
          "jsonValue": "[\"62e90394-69f5-4237-9190-012177145e10\",\"f28a1f50-f6e7-4571-818b-6a12f2af6b6c\",\"29232cdf-9323-42fd-ade2-1d097af3e4de\",\"b1be1c3e-b65d-4f19-8427-f6fa0d97feb9\",\"194ae4cb-b126-40b2-bd5b-6091b380977d\",\"729827e3-9c14-49f7-bb1b-9608f156bbb8\",\"b0f54661-2d74-4c50-afa3-1ec803f12efe\",\"fe930be7-5e62-47db-91af-98c3a49a38b1\",\"c4e39bd9-1100-46d3-8c65-fb160da0071f\"]"
        },
        {
          "settingId": "e1e6c785-039a-4353-b826-100a222bb085",
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "settingId": "af9bd2da-1716-4778-b06c-8f6970ecd868",
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "overwriteAllowed": false,
          "jsonValue": "\"OR\""
        },
        {
          "settingId": "f68ae11b-fea1-4674-a9df-2bf164173eea",
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
    },
    "version": 1
  },
  "tenantId": "6b0e46f8-4e82-4e58-8c0e-c9fe934c011d",
  "settings": [
    {
      "settingId": "82d2bbb1-a6dc-4c8d-90c1-60387a492eda",
      "valueType": "string",
      "displayName": "DisplayName",
      "overwriteAllowed": false,
      "jsonValue": "\"Baseline – Require MFA for Admins\""
    },
    {
      "settingId": "bb898877-c130-42f0-9d2f-ec92701bfee7",
      "valueType": "string",
      "displayName": "State",
      "overwriteAllowed": false,
      "jsonValue": "\"enabledForReportingButNotEnforced\""
    }
  ],
  "status": "inProgress"
}
```
