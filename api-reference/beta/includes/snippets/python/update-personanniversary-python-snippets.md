---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonAnnualEvent()
request_body.setAllowedAudiences(AllowedAudiences('contacts'))


request_config = PersonAnnualEventRequestBuilderPatchRequestConfiguration(
request_config = PersonAnnualEventRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.profile.anniversaries_by_id('personAnnualEvent-id').patch(request_body, headers=)


```