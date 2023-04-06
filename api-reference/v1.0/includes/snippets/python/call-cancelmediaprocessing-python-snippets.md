---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelMediaProcessingPostRequestBody()
request_body.setClientContext('clientContext-value')


request_config = CancelMediaProcessingRequestBuilderPostRequestConfiguration(
request_config = CancelMediaProcessingRequestBuilderPostRequestConfiguration(query_params=)


result = await client.communications.calls_by_id('call-id').cancelMediaProcessing.post(request_body, headers=)


```