---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
additionalData = [
'graphlearn_courses' => request_body = Graphlearn_courses()
		request_body.setCourseId('123')

		request_body.setCourseName('New Managers')

		request_body.setCourseType('Online')


request_body.setGraphlearn_courses($graphlearn_courses)

];
request_body.setAdditionalData(additionalData)




result = await client.groups_by_id('group-id').patch(request_body)


```