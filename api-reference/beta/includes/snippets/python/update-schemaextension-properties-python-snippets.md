---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = User();
additionalData = [
'ext55gb1l09_msLearnCourses' => requestBody = Ext55gb1l09_msLearnCourses();
		requestBody.setCourseType('Admin');


requestBody.setExt55gb1l09_msLearnCourses($ext55gb1l09_msLearnCourses);

];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.usersById('user-id').patch(requestBody);


```