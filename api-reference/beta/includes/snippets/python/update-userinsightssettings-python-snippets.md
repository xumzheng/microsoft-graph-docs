---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UserInsightsSettings();
requestBody.setIsEnabled(false);



requestResult = graphServiceClient.usersById('user-id').settings().itemInsights().patch(requestBody);


```