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

## Examples

### Example 1: Update the entire peopleInsightSettings object of the signed-in user

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_peopleinsightsettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/peopleInsights
Content-type: application/json

{
    "isEnabled": true
}
```

#### Response

The following is an example of the response.
<!-- {
  "blockType": "response",
  "name": "put_peopleinsightsettings"
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
  "name": "patch_peopleinsightsettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/peopleInsights
Content-type: application/json

{
  "isEnabled": false
}
```

#### Response

The following is an example of the response.
<!-- {
  "blockType": "response",
  "name": "patch_peopleinsightsettings"
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


