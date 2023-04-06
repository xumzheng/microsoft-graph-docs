---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalConnection()
request_body.setName('Contoso HR Service Tickets')

request_body.setDescription('Connection to index HR service tickets')


request_config = ExternalConnectionRequestBuilderPatchRequestConfiguration(
request_config = ExternalConnectionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.external.connections_by_id('externalConnection-id').patch(request_body, headers=)


```