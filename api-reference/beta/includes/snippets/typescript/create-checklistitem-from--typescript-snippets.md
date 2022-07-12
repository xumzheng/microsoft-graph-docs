---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChecklistItem = {
	displayName : "Final sign-off from the team",
};

const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").tasksById("baseTask-id").checklistItems.post(requestBody);
}


```