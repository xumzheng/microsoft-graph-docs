---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerRosterMember();
requestBody.set@odatatype('#microsoft.graph.plannerRosterMember');

requestBody.setUserId('String');



result = awaitclient.planner().rostersById('plannerRoster-id').members().post(requestBody);


```