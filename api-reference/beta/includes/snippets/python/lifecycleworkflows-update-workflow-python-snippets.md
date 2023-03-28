---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Workflow();
$requestBody.setDescription('Configure new hire tasks for onboarding employees on their first day');

$requestBody.setDisplayName('Australia Onboard new hire employee');

$requestBody.setIsEnabled(true);

$requestBody.setIsSchedulingEnabled(false);



$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').patch($requestBody);


```