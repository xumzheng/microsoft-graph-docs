---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
additionalData = [
'extkmpdyld2_graphLearnCourses' => request_body = Extkmpdyld2_graphLearnCourses()
		request_body.setCourseType('Instructor-led')

		request_body.setCourseId(null)


request_body.setExtkmpdyld2_graphLearnCourses($extkmpdyld2_graphLearnCourses)

];
request_body.setAdditionalData(additionalData)




result = await client.users_by_id('user-id').patch(request_body)


```