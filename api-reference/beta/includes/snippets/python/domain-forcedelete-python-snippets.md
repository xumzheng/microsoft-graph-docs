---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForceDeletePostRequestBody()
request_body.setDisableUserAccounts(true)


request_config = ForceDeleteRequestBuilderPostRequestConfiguration(
request_config = ForceDeleteRequestBuilderPostRequestConfiguration(query_params=)


await client.domains_by_id('domain-id').forceDelete.post(request_body, headers=)


```