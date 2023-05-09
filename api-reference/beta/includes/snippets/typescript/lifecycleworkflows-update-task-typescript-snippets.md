---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Task = {
	description : "Add user to selected groups",
	displayName : "Update marketing day 1 add users to Group set up",
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").tasksById("task-id").patch(requestBody);
}


```