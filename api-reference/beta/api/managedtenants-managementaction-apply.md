---
title: "managementAction: apply"
description: "Applies a management action against a specific managed tenant. By performing this operation the appropriate configurations will be made and policies created. As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: apiPageType
---

# managementAction: apply
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Applies a management action against a specific managed tenant. By performing this operation the appropriate configurations will be made and policies created. As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role.

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
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
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
|tenantGroupId|String|The identifier for the tenant group.|
|managementTemplateId|The identifier of the [management template](../resources/managedtenants-managementtemplate.md).|
|includeAllUsers|Boolean|A flag indicating whether or not all users should be included when applying the management action if supported.|
|includeGroups|String collection|A collection of identifiers for Azure Active Directory groups that will be used for the inclusion assignment if supported.|
|excludeGroups|String collection|A collection of identifiers for Azure Active Directory groups that will be used for the exclusion assignment if supported.|

## Response

If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "managementactionthis.apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json
Content-length: 212

{
  "tenantId": "6b0e46f8-4e82-4e58-8c0e-c9fe934c011d",
  "tenantGroupId": "afddf5fe-42b1-461f-9472-91507eb71486",
  "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
  "includeAllUsers": false,
  "includeGroups": [],
  "excludeGroups": []
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementaction-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementaction-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementaction-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/managementaction-apply-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/managementaction-apply-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#managementActionDeploymentStatus",
  "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
  "managementTemplateVersion": 1,
  "managementActionId": "759fb1b5-b1f4-4789-964b-bb8ce5a9f0e6",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "4a1c5d34-c2f7-4fd5-a7b5-4bedd95bb8f9",
      "status": "completed",
      "deployedPolicyId": "cd57047b-c93c-48d4-81f8-97f2a5c84434",
      "lastDeploymentDateTime": "2021-05-14T17:46:54.2140431Z",
      "includeAllUsers": true
    }
  ]
}
```
