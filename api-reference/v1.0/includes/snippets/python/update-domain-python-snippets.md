---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Domain()
request_body.setIsDefault(true)

request_body.setSupportedServices(['Email', 'OfficeCommunicationsOnline', ])


request_config = DomainRequestBuilderPatchRequestConfiguration(
request_config = DomainRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.domains_by_id('domain-id').patch(request_body, headers=)


```