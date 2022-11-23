---
title: "Update peopleInsightSettings"
description: "Update the peopleInsights settings of a user."
author: "arunjose"
ms.localizationpriority: medium
ms.prod: "users"
doc_type: apiPageType
---

# Update peopleInsightSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update some or all of the properties of a [peopleInsightSettings](../resources/peopleInsightSettings.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission Type                   |Permission (from least to most privileged)     |
|----------------------------------|---------------------------------------------- |
|Delegated (work or school account)|User.ReadWrite, User.ReadWrite.All             |
|Delegated (personal account)      |User.ReadWrite, User.ReadWrite.All             |
|Application                       |User.ReadWrite, User.ReadWrite.All             |

## HTTP request

To update all of a user's peopleInsights settings:
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/peopleInsights
```

To update a subset of the properties of a user's peopleInsights settings:
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/peopleInsights
```

## Request headers
| Header       | Value|
|:-----------|:------|
| Authorization  | Bearer {token}. Required.  |
| Content-Type  | application/json. Required.  |

## Request body
 **PUT**: In the request body, supply a [peopleInsightSettings](../resources/peopleinsightsettings.md) object.
 
 **PATCH**: Only supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.
 
## Response

If successful, this method returns a 200 response code and the updated **peopleInsightSettings** object.

## Example

### Example 1: Update the entire peopleInsightSettings object of the signed-in user

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_peopleInsightSettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/peopleInsights
Content-type: application/json

{
    "isEnabled": true
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-peopleinsightsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-peopleinsightsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-peopleinsightsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/put-peopleinsightsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [snippet-not-available](../includes/snippets/snippet-not-available.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/put-peopleinsightsettings-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.
<!-- {
  "blockType": "response",
  "name": "put_peopleInsightSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### Example 2: Update selected properties of the signed-in user

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_peopleInsightSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/peopleInsights
Content-type: application/json

{
  "isEnabled": false
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-peopleinsightsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-peopleinsightsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-peopleinsightsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/patch-peopleinsightsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/patch-peopleinsightsettings-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/patch-peopleinsightsettings-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### Response

The following is an example of the response.
<!-- {
  "blockType": "response",
  "name": "patch_peopleInsightSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update peopleInsightSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


