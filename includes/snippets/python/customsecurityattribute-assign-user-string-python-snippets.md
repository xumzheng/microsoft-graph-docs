---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = User();
customSecurityAttributes = CustomSecurityAttributeValue();
additionalData = [
'Engineering' => customSecurityAttributes = Engineering();
		customSecurityAttributes.set@odatatype('#Microsoft.DirectoryServices.CustomSecurityAttributeValue');

		customSecurityAttributes.setProjectDate('2022-10-01');


customSecurityAttributes.setEngineering($engineering);

];
customSecurityAttributes.setAdditionalData(additionalData);



requestBody.setCustomSecurityAttributes($customSecurityAttributes);


requestResult = graphServiceClient.usersById('user-id').patch(requestBody);


```