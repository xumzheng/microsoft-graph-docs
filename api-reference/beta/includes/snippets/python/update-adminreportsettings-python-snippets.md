---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AdminReportSettings();
requestBody.setDisplayConcealedNames(true);



result = awaitclient.admin().reportSettings().patch(requestBody);


```