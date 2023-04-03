---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = InsightsSettings();
requestBody.setDisabledForGroup('edbfe4fb-ec70-4300-928f-dbb2ae86c981');



result = awaitclient.organizationById('organization-id').settings().itemInsights().patch(requestBody);


```