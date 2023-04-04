---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CustomSecurityAttributeDefinition();
request_body.setAttributeSet('Engineering');

request_body.setDescription('Active projects for user');

request_body.setIsCollection(true);

request_body.setIsSearchable(true);

request_body.setName('Project');

request_body.setStatus('Available');

request_body.setType('String');

request_body.setUsePreDefinedValuesOnly(true);



result = await client.directory().customSecurityAttributeDefinitions().post(request_body);


```