---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Domain()
request_body.isDefault = true

request_body.SupportedServices(['Email', 'OfficeCommunicationsOnline', ])




result = await client.domains_by_id('domain-id').patch(request_body = request_body)


```