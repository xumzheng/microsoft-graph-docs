---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
custom_security_attributes = CustomSecurityAttributeValue()
additionalData = [
'Engineering' => custom_security_attributes = Engineering()
		customSecurityAttributes.@odatatype = '#Microsoft.DirectoryServices.CustomSecurityAttributeValue'

		customSecurityAttributes.numVendors@odatatype = '#Int32'

		customSecurityAttributes.num_vendors = 8


customSecurityAttributes.engineering = engineering

];
customSecurityAttributes.additionaldata(additionalData)



request_body.custom_security_attributes = customSecurityAttributes



result = await client.users_by_id('user-id').patch(request_body = request_body)


```