---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AdminReportSettings();
requestBody.setDisplayConcealedNames(true);



result = await client.admin().reportSettings().patch(requestBody);


```