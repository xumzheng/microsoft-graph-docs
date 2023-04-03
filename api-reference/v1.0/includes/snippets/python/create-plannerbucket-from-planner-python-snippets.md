---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerBucket();
requestBody.setName('Advertising');

requestBody.setPlanId('xqQg5FS2LkCp935s-FIFm2QAFkHM');

requestBody.setOrderHint(' !');



result = awaitclient.planner().buckets().post(requestBody);


```