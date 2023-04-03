---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExternalConnection();
requestBody.setId('contosohr');

requestBody.setName('Contoso HR');

requestBody.setDescription('Connection to index Contoso HR system');



result = awaitclient.external().connections().post(requestBody);


```