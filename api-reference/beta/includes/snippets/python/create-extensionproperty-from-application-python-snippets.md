---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExtensionProperty();
requestBody.setName('jobGroup');

requestBody.setDataType('String');

requestBody.setTargetObjects(['User', ]);



result = awaitclient.applicationsById('application-id').extensionProperties().post(requestBody);


```