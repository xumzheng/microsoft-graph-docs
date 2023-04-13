---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
additionalData = [
'graphlearn_courses' => request_body = Graphlearn_courses()
		request_body.courseId = '123'

		request_body.courseName = 'New Managers'

		request_body.courseType = 'Online'


request_body.graphlearn_courses = graphlearn_courses

];
request_body.additionaldata(additionalData)





result = await client.groups_by_id('group-id').patch(request_body = request_body)


```