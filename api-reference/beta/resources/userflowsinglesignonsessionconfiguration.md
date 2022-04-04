---
title: "userFlowSingleSignOnSessionConfiguration resource type"
description: "Configure the single-sign on session (SSO) behavior of the Azure AD B2C user flows"
author: "nickgmicrosoft"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowSingleSignOnSessionConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Defines single sign-on (SSO) behavior for an Azure AD B2C user flow. SSO adds security and convenience when users sign in across applications.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isSessionLifetimeAbsolute|Boolean|Indicates how a session is extended by the session lifetime setting or the Keep me signed in (KMSI) setting. `true` Indicates that the user is forced to re-authenticate after the time period specified. `false`  indicates that the session is extended every time the user performs a cookie-based authentication (default).|
|sessionLifetimeInMinutes|Int32|The amount of time the Azure AD B2C session cookie is stored on the user's browser after successful authentication. You can set the session lifetime up to 1440 minutes (24 hours).|
|isKeepMeSignedInEnabled|Boolean|Represents whenever "keep me sign in" is enabled or not, when `false`, "keepMeSignedInDays" is not modifiable.|
<!-- |keepAliveInDays|Int32|The amount of days to keep the session active for local accounts.| -->
|keepMeSignedInDays|Int32|The amount of days to keep the session active for local accounts.|
|sessionScope|userFlowSingleSignOnConfigurationScope|Governs the scope of a user's single sign on experience and whether a user session applies on the entire tenant, per application, per policy, or is disabled. The possible values are: `tenant`, `application`, `policy`, or `disabled`. Default value is `tenant`.|
|enforceIdTokenHintOnLogout|Boolean|Enforces the presence of a previously issued ID Token passed to the logout endpoint. Default value is `false`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowSingleSignOnSessionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowSingleSignOnSessionConfiguration",
  "isSessionLifetimeAbsolute": "Boolean",
  "sessionLifetimeInMinutes": "Integer",
  "isKeepMeSignedInEnabled": "Boolean",
  "keepMeSignedInDays": "Integer",
  "sessionScope": "String",
  "enforceIdTokenHintOnLogout": "Boolean"
}
```