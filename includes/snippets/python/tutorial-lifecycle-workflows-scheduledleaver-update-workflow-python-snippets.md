---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Workflow();
requestBody.setIsEnabled(true);

requestBody.setIsSchedulingEnabled(true);



requestResult = graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').patch(requestBody);


```