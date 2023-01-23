---
title: "Create learningCourseActivity"
description: "Create a new learningCourseActivity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Create learningCourseActivity
Namespace: microsoft.graph



Create a new [learningCourseActivity](../resources/learningcourseactivity.md) object.

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
POST /employeeExperience/learningCourseActivities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [learningCourseActivity](../resources/learningcourseactivity.md) object.

You can specify the following properties when creating a **learningCourseActivity**.

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

If successful, this method returns a `201 Created` response code and a [learningCourseActivity](../resources/learningcourseactivity.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_learningcourseactivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/employeeExperience/learningCourseActivities
Content-Type: application/json

{
  "@odata.type": "#microsoft.vivaLearning.learningCourseActivity",
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
  "truncated": true,
  "@odata.type": "microsoft.vivaLearning.learningCourseActivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.vivaLearning.learningCourseActivity",
  "externalcourseActivityId": "String",
  "learningProviderId": "String",
  "learningContentId": "String",
  "learnerUserId": "String",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "completionPercentage": "Integer"
}
```

