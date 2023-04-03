---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDisplayName('New Managers March 2017');

requestBody.setDescription('New Managers training course for March 2017');

requestBody.setGroupTypes(['Unified', ]);

requestBody.setMailEnabled(true);

requestBody.setMailNickname('newMan201703');

requestBody.setSecurityEnabled(false);

additionalData = [
'graphlearn_courses' => requestBody = Graphlearn_courses();
	requestBody.setCourseId('123');

	requestBody.setCourseName('New Managers');

	requestBody.setCourseType('Online');


requestBody.setGraphlearn_courses($graphlearn_courses);

];
requestBody.setAdditionalData(additionalData);




result = await client.groups().post(requestBody);


```