---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Domain()
request_body.setIsDefault(true)

request_body.setSupportedServices(['Email', 'OfficeCommunicationsOnline', ])



result = await client.domainsById('domain-id').patch(request_body)


```