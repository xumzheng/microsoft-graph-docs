---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AdminReportSettings();
requestBody.setDisplayConcealedNames(true);



requestResult = graphServiceClient.admin().reportSettings().patch(requestBody);


```