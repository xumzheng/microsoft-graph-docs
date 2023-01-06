---
title: "Update landingPageDetail"
description: "Update the properties of a landingPageDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Update landingPageDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [landingPageDetail](../resources/landingpagedetail.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/attackSimulation/landingPages/{landingPageId}/details/{landingPageDetailId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|content|String|**TODO: Add Description** Optional.|
|language|String|**TODO: Add Description** Optional.|
|isDefaultLangauge|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [landingPageDetail](../resources/landingpagedetail.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_landingpagedetail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/attackSimulation/landingPages/{landingPageId}/details/{landingPageDetailId}
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.landingPageDetail",
  "content": "String",
  "language": "String",
  "isDefaultLangauge": "Boolean"
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
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.landingPageDetail",
  "id": "d495efad-a51b-d557-7ce3-ff1c8ed7db8a",
  "content": "String",
  "language": "String",
  "isDefaultLangauge": "Boolean"
}
```

