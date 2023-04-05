---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonInterest()
request_body.setCategories(['Sports', ])



result = await client.me_profile_interestsby_id('personInterest-id').patch(request_body)


```