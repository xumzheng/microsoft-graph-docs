---
title: "templateAction resource type"
description: "Represents an action that can be performed to configure Microsoft 365 services."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# templateAction resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an action that can be performed to configure Microsoft 365 services.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description for the template action.|
|displayName|String|The display name for the template action.|
|service|String|Indicates the Microsoft 365 service where the template action can be performed. Possible values include: `AAD` and `Intune`|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|The collection of settings associated with the template action.|
|templateActionId|String|The unique identifier for the template action.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|licenses|[licenseDetails](../resources/licensedetails.md)|The license that is required for the template action to be performed.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateAction",
  "templateActionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
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
      "settingId": "0f52c9ff-1ec0-41f2-b5c2-eb661de2f46a",
      "valueType": "string",
      "displayName": "DisplayName",
      "overwriteAllowed": false,
      "jsonValue": "\"Baseline – Require MFA for Admins\""
    },
    {
      "settingId": "f2038fde-483c-4df2-a3af-448e8dc881f4",
      "valueType": "string",
      "displayName": "State",
      "overwriteAllowed": false,
      "jsonValue": "\"enabledForReportingButNotEnforced\""
    },
    {
      "settingId": "34e048f3-a2dc-408b-a246-4914af178062",
      "valueType": "stringCollection",
      "displayName": "ClientAppTypes",
      "overwriteAllowed": false,
      "jsonValue": "[\"All\"]"
    },
    {
      "settingId": "38512fb8-b8ab-45cc-9296-ff28ca5c4fcf",
      "valueType": "stringCollection",
      "displayName": "IncludeApplications",
      "overwriteAllowed": false,
      "jsonValue": "[\"All\"]"
    },
    {
      "settingId": "20b2d2b6-4c5b-4c18-b2c4-ad8e70fb764d",
      "valueType": "stringCollection",
      "displayName": "IncludeRoles",
      "overwriteAllowed": false,
      "jsonValue": "[\"62e90394-69f5-4237-9190-012177145e10\",\"f28a1f50-f6e7-4571-818b-6a12f2af6b6c\",\"29232cdf-9323-42fd-ade2-1d097af3e4de\",\"b1be1c3e-b65d-4f19-8427-f6fa0d97feb9\",\"194ae4cb-b126-40b2-bd5b-6091b380977d\",\"729827e3-9c14-49f7-bb1b-9608f156bbb8\",\"b0f54661-2d74-4c50-afa3-1ec803f12efe\",\"fe930be7-5e62-47db-91af-98c3a49a38b1\",\"c4e39bd9-1100-46d3-8c65-fb160da0071f\"]"
    },
    {
      "settingId": "8dc0582b-ccb1-4466-ac75-fb7e3191a686",
      "valueType": "stringCollection",
      "displayName": "IncludeLocations",
      "overwriteAllowed": false,
      "jsonValue": "[\"All\"]"
    },
    {
      "settingId": "09ccf4f9-f3c5-4e3a-9686-1b1a5a74f336",
      "valueType": "string",
      "displayName": "GrantControls.Operator",
      "overwriteAllowed": false,
      "jsonValue": "\"OR\""
    },
    {
      "settingId": "c5367659-4764-4af1-98e2-9ba2e88b4a28",
      "valueType": "stringCollection",
      "displayName": "GrantControls.BuiltInControls",
      "overwriteAllowed": false,
      "jsonValue": "[\"mfa\"]"
    }
  ]
}
```
