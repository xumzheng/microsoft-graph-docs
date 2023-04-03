---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Workflow();
requestBody.setIsEnabled(true);

requestBody.setIsSchedulingEnabled(true);



result = awaitclient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').patch(requestBody);


```