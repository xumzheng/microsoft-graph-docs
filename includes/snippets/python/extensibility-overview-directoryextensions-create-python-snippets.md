---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExtensionProperty()
request_body.name = 'jobGroupTracker'

request_body.dataType = 'String'

request_body.TargetObjects(['User', ])




result = await client.applications_by_id('application-id').extensionProperties.post(request_body = request_body)


```