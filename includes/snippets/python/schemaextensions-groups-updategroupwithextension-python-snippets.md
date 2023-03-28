---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Group();
$additionalData = [
'graphlearn_courses' => $requestBody = new Graphlearn_courses();
$		requestBody.setCourseId('123');

$		requestBody.setCourseName('New Managers');

$		requestBody.setCourseType('Online');


$requestBody.setGraphlearn_courses($graphlearn_courses);

];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.groupsById('group-id').patch($requestBody);


```