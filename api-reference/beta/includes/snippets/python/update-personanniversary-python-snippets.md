---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonAnnualEvent()
request_body.AllowedAudiences(AllowedAudiences('contacts'))



request_configuration = PersonAnnualEventRequestBuilderPatchRequestConfiguration(
)


result = await client.me.profile.anniversaries_by_id('personAnnualEvent-id').patch(request_body = request_body)


```