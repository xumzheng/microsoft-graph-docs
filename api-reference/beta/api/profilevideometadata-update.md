---
title: "Update profileVideoMetadata"
description: "Update the properties of a profileVideoMetadata object."
author: "kevinbellinger"
ms.localizationpriority: medium
ms.prod: "people"
doc_type: apiPageType
---

# Update profileVideoMetadata
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [profileVideoMetadata](../resources/profilevideometadata.md) object in a user's [profile](../resources/profile.md).

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|User.ReadWrite|
|Delegated (personal Microsoft account)|User.ReadWrite|
|Application|User.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/profileVideoMetadata
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|profileVideoUrl|String|Provides the url to the actual profile video file Optional.|



## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_profilevideometadata"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/profileVideoMetadata
Content-Type: application/json

{
  "profileVideoUrl": "https://graph.microsoft.com/v1.0/users/{userId}/drive/items/aHR0cHM6Ly9taWNyb3NvZnQtbXkuc2hhcmV"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```

