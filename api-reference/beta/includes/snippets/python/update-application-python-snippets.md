---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
request_body.displayName = 'New display name'



request_configuration = ApplicationRequestBuilderPatchRequestConfiguration(
)


result = await client.applications_by_id('application-id').patch(request_body = request_body)


```