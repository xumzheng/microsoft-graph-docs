---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserInsightsSettings();
requestBody.setIsEnabled(false);



result = awaitclient.usersById('user-id').settings().itemInsights().patch(requestBody);


```