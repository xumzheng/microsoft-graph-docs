---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ClearPresencePostRequestBody();
requestBody.setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');



awaitclient.usersById('user-id').presence().clearPresence().post(requestBody);


```