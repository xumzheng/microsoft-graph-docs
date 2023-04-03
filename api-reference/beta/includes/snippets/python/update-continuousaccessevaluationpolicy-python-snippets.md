---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ContinuousAccessEvaluationPolicy();
requestBody.set@odatatype('#microsoft.graph.continuousAccessEvaluationPolicy');

requestBody.setMigrate(true);



result = await client.identity().continuousAccessEvaluationPolicy().patch(requestBody);


```