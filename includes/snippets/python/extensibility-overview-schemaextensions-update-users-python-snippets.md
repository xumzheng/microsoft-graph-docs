---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
additionalData = [
'extkmpdyld2_graphLearnCourses' => requestBody = Extkmpdyld2_graphLearnCourses();
		requestBody.setCourseType('Instructor-led');

		requestBody.setCourseId(null);


requestBody.setExtkmpdyld2_graphLearnCourses($extkmpdyld2_graphLearnCourses);

];
requestBody.setAdditionalData(additionalData);




result = await client.usersById('user-id').patch(requestBody);


```