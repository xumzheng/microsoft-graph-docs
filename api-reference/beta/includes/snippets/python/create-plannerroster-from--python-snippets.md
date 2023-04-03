---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerRoster();
requestBody.set@odatatype('#microsoft.graph.plannerRoster');



result = awaitclient.planner().rosters().post(requestBody);


```