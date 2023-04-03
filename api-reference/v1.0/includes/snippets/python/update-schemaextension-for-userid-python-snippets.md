---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
additionalData = [
'ext55gb1l09_msLearnCourses' => requestBody = Ext55gb1l09_msLearnCourses();
		requestBody.setCourseType('Admin');


requestBody.setExt55gb1l09_msLearnCourses($ext55gb1l09_msLearnCourses);

];
requestBody.setAdditionalData(additionalData);




result = await client.usersById('user-id').patch(requestBody);


```