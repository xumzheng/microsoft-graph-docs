---
title: "Get profileVideoMetadata"
description: "Retrieve the properties and relationships of a profileVideoMetadata object."
author: "kevinbellinger"
ms.localizationpriority: medium
ms.prod: "people"
doc_type: apiPageType
---

# Get profileVideoMetadata
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve the properties and relationships of a [profileVideoMetadata](../resources/profilevideometadata.md) object from a user's [profile](../resources/profile.md).

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|User.Read, User.ReadWrite, User.Read.All|
|Delegated (personal Microsoft account)|User.Read, User.ReadWrite, User.Read.All|
|Application|User.Read.All, User.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/profileVideoMetadata
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [profileVideoMetadata](../resources/profilevideometadata.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_profilevideometadata"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/profileVideoMetadata
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileVideoMetadata"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.profileVideoMetadata",
    "id": "9e798570-5fab-43fb-152a-3de32e83c8ce",
    "allowedAudiences": "organization",
    "inference": null,
    "createdDateTime": "2020-07-06T06:34:12.2294868Z",
    "createdBy": {
      "application": null,
      "device": null,
      "user": {
        "displayName": "Innocenty Popov",
        "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
      }
    },
    "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
    "lastModifiedBy": {
      "application": null,
      "device": null,
      "user": {
        "displayName": "Innocenty Popov",
        "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
      }
    },
    "source": null,
    "isSearchable": "true",
    "profileVideoUrl": "https://graph.microsoft.com/v1.0/users/{userId}/drive/items/01UVTC6G45XUCMK4BMYNH2HUKQ5CMM26K7"
  }
}
```

