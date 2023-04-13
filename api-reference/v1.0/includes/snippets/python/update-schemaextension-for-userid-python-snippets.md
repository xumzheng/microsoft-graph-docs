---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
additionalData = [
'ext55gb1l09_msLearnCourses' => request_body = Ext55gb1l09_msLearnCourses()
		request_body.courseType = 'Admin'


request_body.ext55gb1l09_msLearnCourses = ext55gb1l09_msLearnCourses

];
request_body.additionaldata(additionalData)





result = await client.users_by_id('user-id').patch(request_body = request_body)


```