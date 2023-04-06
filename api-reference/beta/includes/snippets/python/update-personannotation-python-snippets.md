---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonAnnotation()
request_body.setAllowedAudiences(AllowedAudiences('organization'))


request_config = PersonAnnotationRequestBuilderPatchRequestConfiguration(
request_config = PersonAnnotationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.users_by_id('user-id').profile.notes_by_id('personAnnotation-id').patch(request_body, headers=)


```