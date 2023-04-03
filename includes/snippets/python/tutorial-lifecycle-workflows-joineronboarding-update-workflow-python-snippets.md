---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Workflow();
requestBody.setIsEnabled(true);

requestBody.setIsSchedulingEnabled(true);



result = await client.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').patch(requestBody);


```