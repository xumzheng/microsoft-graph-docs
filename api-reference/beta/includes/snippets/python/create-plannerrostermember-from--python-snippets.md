---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PlannerRosterMember();
requestBody.set@odatatype('#microsoft.graph.plannerRosterMember');

requestBody.setUserId('String');



requestResult = graphServiceClient.planner().rostersById('plannerRoster-id').members().post(requestBody);


```