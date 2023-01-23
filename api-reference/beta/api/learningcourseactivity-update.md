---
title: "Update learningCourseActivity"
description: "Update the properties of a learningCourseActivity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Update learningCourseActivity
Namespace: microsoft.graph



Update the properties of a [learningCourseActivity](../resources/learningcourseactivity.md) object.

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
PATCH /employeeExperience/learningCourseActivities/{learningCourseActivityId}
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
|externalcourseActivityId|String|**TODO: Add Description** Optional.|
|learningProviderId|String|**TODO: Add Description** Optional.|
|learningContentId|String|**TODO: Add Description** Required.|
|learnerUserId|String|**TODO: Add Description** Required.|
|status|courseStatus|**TODO: Add Description**. The possible values are: `notStarted`, `inProgress`, `completed`, `unknownFutureValue`. Optional.|
|completedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|completionPercentage|Int32|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [learningCourseActivity](../resources/learningcourseactivity.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_learningcourseactivity"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/employeeExperience/learningCourseActivities/{learningCourseActivityId}
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.learningCourseActivity",
  "externalcourseActivityId": "String",
  "learningProviderId": "String",
  "learningContentId": "String",
  "learnerUserId": "String",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "completionPercentage": "Integer"
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
  "@odata.type": "#microsoft.graph.learningCourseActivity",
  "externalcourseActivityId": "String",
  "learningProviderId": "String",
  "learningContentId": "String",
  "learnerUserId": "String",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "completionPercentage": "Integer"
}
```

