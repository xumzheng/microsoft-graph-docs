---
title: "Get learningCourseActivity"
description: "Read the properties and relationships of a learningCourseActivity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Get learningCourseActivity
Namespace: microsoft.graph



Read the properties and relationships of a [learningCourseActivity](../resources/learningcourseactivity.md) object.

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
GET /employeeExperience/learningCourseActivities/{learningCourseActivityId}
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

If successful, this method returns a `200 OK` response code and a [learningCourseActivity](../resources/learningcourseactivity.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_learningcourseactivity"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/employeeExperience/learningCourseActivities/{learningCourseActivityId}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.vivaLearning.learningCourseActivity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.vivaLearning.learningCourseActivity",
    "externalcourseActivityId": "String",
    "learningProviderId": "String",
    "learningContentId": "String",
    "learnerUserId": "String",
    "status": "String",
    "completedDateTime": "String (timestamp)",
    "completionPercentage": "Integer"
  }
}
```

