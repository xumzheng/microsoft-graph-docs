---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
customSecurityAttributes = CustomSecurityAttributeValue();
additionalData = [
'Engineering' => customSecurityAttributes = Engineering();
		customSecurityAttributes.set@odatatype('#Microsoft.DirectoryServices.CustomSecurityAttributeValue');

		customSecurityAttributes.setNumVendors@odatatype('#Int32');

		customSecurityAttributes.setNumVendors(4);


customSecurityAttributes.setEngineering($engineering);

];
customSecurityAttributes.setAdditionalData(additionalData);



requestBody.setCustomSecurityAttributes($customSecurityAttributes);


result = await client.usersById('user-id').patch(requestBody);


```