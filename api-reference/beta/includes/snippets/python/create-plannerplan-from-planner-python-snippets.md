---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PlannerPlan();
container = PlannerPlanContainer();
container.setUrl('https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874');


requestBody.setContainer($container);
requestBody.setTitle('title-value');



result = await client.planner().plans().post(requestBody);


```