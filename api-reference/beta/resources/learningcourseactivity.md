---
title: "learningCourseActivity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# learningCourseActivity resource type

Namespace: microsoft.graph



**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List learningCourseActivities](../api/employeeexperienceuser-list-learningcourseactivities.md)|[learningCourseActivity](../resources/learningcourseactivity.md) collection|Get a list of the [learningCourseActivity](../resources/learningcourseactivity.md) objects and their properties.|
|[Create learningCourseActivity](../api/employeeexperienceuser-post-learningcourseactivities.md)|[learningCourseActivity](../resources/learningcourseactivity.md)|Create a new [learningCourseActivity](../resources/learningcourseactivity.md) object.|
|[Get learningCourseActivity](../api/learningcourseactivity-get.md)|[learningCourseActivity](../resources/learningcourseactivity.md)|Read the properties and relationships of a [learningCourseActivity](../resources/learningcourseactivity.md) object.|
|[Update learningCourseActivity](../api/learningcourseactivity-update.md)|[learningCourseActivity](../resources/learningcourseactivity.md)|Update the properties of a [learningCourseActivity](../resources/learningcourseactivity.md) object.|
|[Delete learningCourseActivity](../api/employeeexperienceuser-delete-learningcourseactivities.md)|None|Delete a [learningCourseActivity](../resources/learningcourseactivity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|completionPercentage|Int32|**TODO: Add Description**|
|externalcourseActivityId|String|**TODO: Add Description**|
|learnerUserId|String|**TODO: Add Description**|
|learningContentId|String|**TODO: Add Description**|
|learningProviderId|String|**TODO: Add Description**|
|status|courseStatus|**TODO: Add Description**.The possible values are: `notStarted`, `inProgress`, `completed`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningCourseActivity",
  "openType": false
}
-->
``` json
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

