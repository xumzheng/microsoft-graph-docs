---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EvaluateDynamicMembershipPostRequestBody()
request_body.setMemberId('319b41e8-d9e4-42f8-bdc9-741113f48b33')



result = await client.groupsby_id('group-id').evaluateDynamicMembership.post(request_body)


```