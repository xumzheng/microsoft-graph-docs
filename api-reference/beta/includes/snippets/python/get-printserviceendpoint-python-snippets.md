---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PrintServiceEndpointRequestBuilderGetRequestConfiguration(
)


result = await client.print.services_by_id('printService-id').endpoints_by_id('printServiceEndpoint-id').get()


```