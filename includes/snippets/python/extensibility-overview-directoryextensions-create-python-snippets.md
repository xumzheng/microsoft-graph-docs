---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExtensionProperty();
requestBody.setName('jobGroupTracker');

requestBody.setDataType('String');

requestBody.setTargetObjects(['User', ]);



result = await client.applicationsById('application-id').extensionProperties().post(requestBody);


```