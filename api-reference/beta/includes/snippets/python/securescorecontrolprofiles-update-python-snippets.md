---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SecureScoreControlProfile();
requestBody.setControlStateUpdates('controlStateUpdates-value');



result = await client.security().secureScoreControlProfilesById('secureScoreControlProfile-id').patch(requestBody);


```