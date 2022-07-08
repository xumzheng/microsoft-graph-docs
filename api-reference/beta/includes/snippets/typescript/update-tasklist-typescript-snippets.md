---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BaseTaskList = {
	"@odata.type" : "#microsoft.graph.taskList",
	displayName : "Travel Plan",
};

const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").patch(requestBody);
}


```