---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
additionalData = [
'extkmpdyld2_graphLearnCourses' => request_body = Extkmpdyld2_graphLearnCourses()
		request_body.courseType = 'Instructor-led'

		request_body.courseId=null


request_body.extkmpdyld2_graphLearnCourses = extkmpdyld2_graphLearnCourses

];
request_body.additionaldata(additionalData)




request_configuration = UserRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').patch(request_body = request_body)


```