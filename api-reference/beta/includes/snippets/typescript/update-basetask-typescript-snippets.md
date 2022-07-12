---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BaseTask = {
	"@odata.type" : "#microsoft.graph.task",
	textBody : "String",
	bodyLastModifiedDateTime : new Date("String (timestamp)"),
	completedDateTime : new Date("String (timestamp)"),
	dueDateTime : {
		additionalData : {
			"@odata.type" : "microsoft.graph.dateTimeTimeZone",
		},
	},
	startDateTime : {
		additionalData : {
			"@odata.type" : "microsoft.graph.dateTimeTimeZone",
		},
	},
	importance : "String",
	recurrence : {
		additionalData : {
			"@odata.type" : "microsoft.graph.patternedRecurrence",
		},
	},
	displayName : "String",
	status : "String",
	viewpoint : {
		additionalData : {
			"@odata.type" : "microsoft.graph.taskViewpoint",
		},
	},
};

const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").tasksById("baseTask-id").patch(requestBody);
}


```