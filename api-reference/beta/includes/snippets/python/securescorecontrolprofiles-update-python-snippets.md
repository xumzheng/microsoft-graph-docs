---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SecureScoreControlProfile();
request_body.setControlStateUpdates('controlStateUpdates-value');



result = await client.security().secureScoreControlProfilesById('secureScoreControlProfile-id').patch(request_body);


```