---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PlannerRoster();
requestBody.set@odatatype('#microsoft.graph.plannerRoster');



requestResult = graphServiceClient.planner().rosters().post(requestBody);


```