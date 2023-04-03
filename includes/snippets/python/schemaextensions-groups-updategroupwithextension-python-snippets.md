---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Group();
additionalData = [
'graphlearn_courses' => requestBody = Graphlearn_courses();
		requestBody.setCourseId('123');

		requestBody.setCourseName('New Managers');

		requestBody.setCourseType('Online');


requestBody.setGraphlearn_courses($graphlearn_courses);

];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.groupsById('group-id').patch(requestBody);


```