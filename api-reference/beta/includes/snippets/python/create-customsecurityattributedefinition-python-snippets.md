---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CustomSecurityAttributeDefinition();
requestBody.setAttributeSet('Engineering');

requestBody.setDescription('Target completion date');

requestBody.setIsCollection(false);

requestBody.setIsSearchable(true);

requestBody.setName('ProjectDate');

requestBody.setStatus('Available');

requestBody.setType('String');

requestBody.setUsePreDefinedValuesOnly(false);



result = awaitclient.directory().customSecurityAttributeDefinitions().post(requestBody);


```