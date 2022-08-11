---
title: "Update b2cIdentityUserFlow"
description: "Update the properties of a b2cIdentityUserFlow object."
author: "jkdouglas"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update b2cIdentityUserFlow

Namespace: microsoft.graph

Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)|IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)| Not supported.|
|Application|IdentityUserFlow.ReadWrite.All|

The work or school account needs to belong to one of the following roles:

* Global administrator
* External Identity User Flow administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.

The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).


|Property|Type|Description|
|:---|:---|:---|
|userFlowType|userFlowType| The possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`. |
|userFlowTypeVersion|Single| The version of the user flow.|
|apiConnectorConfiguration|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)|Defines which APIs are called at specific points in the user flow. Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector. |
|tokenLifetimeConfiguration|[userFlowTokenLifetimeConfiguration](../resources/userflowtokenlifetimeconfiguration.md)|Configures the lifetime for ID, access, and refresh tokens.|
|authenticationMethods|b2cAuthenticationMethods|The possible values are: `emailWithPassword`, `userName`, `phoneWithOneTimePassword`. Optional.|
|isConditionalAccessEnforced|Boolean|If this is enabled, then B2C user flows will evaluate CA policies after the primary authentication. If the **userFlowMultifactorAuthenticationState** property in the **userFlowMultifactorAuthenticationConfiguration** object is `conditional`, then this property should be `true`.|
|isJavaScriptEnabled|Boolean|Controls whether JavaScript is allowed to run on the HTML pages. |
|multifactorAuthenticationConfiguration|[userFlowMultifactorAuthenticationConfiguration](../resources/userflowmultifactorauthenticationconfiguration.md)| Configure whether MFA is enabled for the user flow.|
|tokenClaimsConfiguration|[userFlowTokenClaimsConfiguration](../resources/userflowtokenclaimsconfiguration.md)|Defines which claims are present in the id, access, or refresh token.|
|passwordComplexityConfiguration|[userFlowPasswordConfiguration](../resources/userflowpasswordconfiguration.md)|This property determines the password complexity of the password the users must satisfy for signup or password reset flows. Optional.|
|isLanguageCustomizationEnabled|Boolean|The property that determines whether language customization is enabled within the B2C user flow. Language customization is not enabled by default for B2C user flows.|
|defaultLanguageTag|String|Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request. This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.|
|singleSignOnSessionConfiguration|[userFlowSingleSignOnSessionConfiguration](../resources/userflowsinglesignonsessionconfiguration.md)|Configures the single sign-on and Keep Me Signed In (KMSI) session behavior of authentications. |

## Response

If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.

## Examples

### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en"
}
```
# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-b2cidentityuserflow-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response

The following is an example of the response.

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
