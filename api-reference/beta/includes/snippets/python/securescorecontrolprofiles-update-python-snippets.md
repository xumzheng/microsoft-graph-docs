---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SecureScoreControlProfile()
request_body.setControlStateUpdates('controlStateUpdates-value')


request_config = SecureScoreControlProfileRequestBuilderPatchRequestConfiguration(
request_config = SecureScoreControlProfileRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.security.secureScoreControlProfiles_by_id('secureScoreControlProfile-id').patch(request_body, headers=)


```