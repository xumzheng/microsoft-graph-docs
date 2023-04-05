---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
additionalData = [
'ext55gb1l09_msLearnCourses' => request_body = Ext55gb1l09_msLearnCourses()
		request_body.setCourseType('Admin')


request_body.setExt55gb1l09_msLearnCourses($ext55gb1l09_msLearnCourses)

];
request_body.setAdditionalData(additionalData)




result = await client.usersby_id('user-id').patch(request_body)


```