---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ResumePostRequestBody = {
	data : {
		operationStatus : CustomTaskExtensionOperationStatus.Completed,
	},
	source : "sample",
	type : "lifecycleEvent",
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").tasksById("task-id").taskProcessingResultsById("taskProcessingResult-id").microsoftGraphIdentityGovernanceResume.post(requestBody);
}


```