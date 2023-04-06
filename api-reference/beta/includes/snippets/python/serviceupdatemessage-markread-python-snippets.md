---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MarkReadPostRequestBody()
request_body.setMessageIds(['MC172851', 'MC167983', ])


request_config = MarkReadRequestBuilderPostRequestConfiguration(
request_config = MarkReadRequestBuilderPostRequestConfiguration(query_params=)


result = await client.admin.serviceAnnouncement.messages.markRead.post(request_body, headers=)


```