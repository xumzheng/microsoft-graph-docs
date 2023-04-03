---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExternalConnection();
requestBody.setId('contosohr');

requestBody.setName('Contoso HR');

requestBody.setDescription('Connection to index Contoso HR system');



result = await client.external().connections().post(requestBody);


```