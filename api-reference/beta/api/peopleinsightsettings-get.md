---
title: "Get peopleInsights settings resource"
description: "Retrieve the properties of a user's peopleInsights settings"
author: "arunjose"
ms.localizationpriority: medium
ms.prod: "users"
doc_type: apiPageType
---

# Get peopleInsightSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the properties of a [peopleInsightsSettings](../resources/peopleinsightsettings.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission Type                   |Permission (from least to most privileged)     |
|----------------------------------|---------------------------------------------- |
|Delegated (work or school account)|User.Read, User.Read.All                        |
|Delegated (personal account)      |User.Read, User.Read.All              |
|Application                       |User.Read, User.Read.All              |

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /settings/peopleInsights
```
## Optional query parameters
You can use `$select` to get specific peopleInsights settings properties, including those that are not returned by default.

For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).

## Request headers
| Header       | Value|
|:-----------|:------|
| Authorization  | Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and [peopleInsightSettings](../resources/peopleinsightsettings.md) object in the response body.

## Example

The following example gets the properties of the signed-in user.

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_peopleinsightsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/peopleInsights
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-peopleinsightsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-peopleinsightsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-peopleinsightsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-peopleinsightsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-peopleinsightsettings-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-peopleinsightsettings-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.peopleInsightSettings",
  "name": "get_peopleInsightSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "isEnabled": true
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get peopleInsights settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


