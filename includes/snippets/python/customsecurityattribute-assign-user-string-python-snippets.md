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
		customSecurityAttributes.set@odatatype('#Microsoft.DirectoryServices.CustomSecurityAttributeValue')

		customSecurityAttributes.setProjectDate('2022-10-01')


customSecurityAttributes.setEngineering($engineering)

];
customSecurityAttributes.setAdditionalData(additionalData)



request_body.setCustomSecurityAttributes($customSecurityAttributes)


result = await client.usersById('user-id').patch(request_body)


```