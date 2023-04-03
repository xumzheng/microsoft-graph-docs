---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Workflow();
requestBody.setDescription('Configure new hire tasks for onboarding employees on their first day');

requestBody.setDisplayName('Australia Onboard new hire employee');

requestBody.setIsEnabled(true);

requestBody.setIsSchedulingEnabled(false);



result = awaitclient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').patch(requestBody);


```