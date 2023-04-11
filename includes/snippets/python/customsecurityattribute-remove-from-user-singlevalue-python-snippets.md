---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
customSecurityAttributes = CustomSecurityAttributeValue()
additionalData = [
'Engineering' => customSecurityAttributes = Engineering()
		customSecurityAttributes.@odatatype = '#Microsoft.DirectoryServices.CustomSecurityAttributeValue'

		customSecurityAttributes.projectDate=null


customSecurityAttributes.Engineering = engineering

];
customSecurityAttributes.additionaldata(additionalData)



request_body.customSecurityAttributes = customSecurityAttributes



result = await client.users_by_id('user-id').patch(request_body = request_body)


```