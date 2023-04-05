---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalConnection()
request_body.setName('Contoso HR Service Tickets')

request_body.setDescription('Connection to index HR service tickets')



result = await client.external.connectionsById('externalConnection-id').patch(request_body)


```