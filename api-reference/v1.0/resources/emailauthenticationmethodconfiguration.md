---
title: "emailAuthenticationMethodConfiguration resource type"
description: "Represents an email OTP authentication methods policy"
author: "mmcla"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: "resourcePageType"
---

# emailAuthenticationMethodConfiguration resource type

Namespace: microsoft.graph

Represents this tenant's email OTP authentication methods policy. Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method. Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication during invitation redemption and self-service sign-up for specific apps in user flows.

Inherits from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[Get emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Read the properties and relationships of an emailAuthenticationMethodConfiguration object.|
|[Update emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Update the properties of an emailAuthenticationMethodConfiguration object.|
|[Delete emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|None|Deletes an emailAuthenticationMethodConfiguration object.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|Determines whether email OTP is usable by external users for authentication. Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`. Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in October 2021.|
|excludeTargets|[excludeTarget](../resources/excludetarget.md) collection|Groups of users that are excluded from the policy.|
|id|String|The authentication method policy identifier. Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Indicates whether this authentication method is enabled or not. Possible values are: `enabled`, `disabled`.|

## Relationships

|Relationship|Type|Description|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection|A collection of groups that are enabled to use the authentication method.|

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "String",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "id": "String (identifier)",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ],
  "state": "String"
}
```
## Example

### Example 1: Update email Authentication Method Configuration Policy

#### Request

The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "allowExternalIdToUseEmailOtp": "default",
    "excludeTargets": [],
    "id": "Email",
    "includeTargets": [],
    "state": "enabled"
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-emailauthenticationmethodconfiguration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-emailauthenticationmethodconfiguration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/update-emailauthenticationmethodconfiguration-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

