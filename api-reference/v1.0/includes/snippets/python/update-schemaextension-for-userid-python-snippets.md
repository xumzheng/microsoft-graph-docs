---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new User();
$additionalData = [
'ext55gb1l09_msLearnCourses' => $requestBody = new Ext55gb1l09_msLearnCourses();
$		requestBody.setCourseType('Admin');


$requestBody.setExt55gb1l09_msLearnCourses($ext55gb1l09_msLearnCourses);

];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.usersById('user-id').patch($requestBody);


```