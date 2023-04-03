---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PlannerRosterMember();
requestBody.set@odatatype('#microsoft.graph.plannerRosterMember');

requestBody.setUserId('String');



result = await client.planner().rostersById('plannerRoster-id').members().post(requestBody);


```