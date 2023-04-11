---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalConnection()
request_body.name = 'Contoso HR Service Tickets'

request_body.description = 'Connection to index HR service tickets'



request_configuration = ExternalConnectionRequestBuilderPatchRequestConfiguration(
)


result = await client.external.connections_by_id('externalConnection-id').patch(request_body = request_body)


```