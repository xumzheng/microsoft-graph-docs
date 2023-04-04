---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ExternalIdentitiesPolicy()
request_body.setAllowExternalIdentitiesToLeave(false)



result = await client.policies.externalIdentitiesPolicy.patch(request_body)


```