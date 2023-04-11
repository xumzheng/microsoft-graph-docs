---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetMemberObjectsPostRequestBody()
request_body.securityEnabledOnly = true



request_configuration = GetMemberObjectsRequestBuilderPostRequestConfiguration(
)


result = await client.directoryObjects_by_id('directoryObject-id').getMemberObjects.post(request_body = request_body)


```