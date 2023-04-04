---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Group()
request_body.setDisplayName('New Managers March 2017')

request_body.setDescription('New Managers training course for March 2017')

request_body.setGroupTypes(['Unified', ])

request_body.setMailEnabled(true)

request_body.setMailNickname('newMan201703')

request_body.setSecurityEnabled(false)

additionalData = [
'graphlearn_courses' => request_body = Graphlearn_courses()
	request_body.setCourseId('123')

	request_body.setCourseName('New Managers')

	request_body.setCourseType('Online')


request_body.setGraphlearn_courses($graphlearn_courses)

];
request_body.setAdditionalData(additionalData)




result = await client.groups.post(request_body)


```