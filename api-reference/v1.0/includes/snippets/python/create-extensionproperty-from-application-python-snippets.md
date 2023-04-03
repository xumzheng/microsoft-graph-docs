---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExtensionProperty();
requestBody.setName('jobGroup');

requestBody.setDataType('String');

requestBody.setTargetObjects(['User', ]);



requestResult = graphServiceClient.applicationsById('application-id').extensionProperties().post(requestBody);


```