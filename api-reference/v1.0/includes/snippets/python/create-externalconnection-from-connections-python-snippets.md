---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ExternalConnection()
request_body.setId('contosohr')

request_body.setName('Contoso HR')

request_body.setDescription('Connection to index Contoso HR system')



result = await client.external.connections.post(request_body)


```