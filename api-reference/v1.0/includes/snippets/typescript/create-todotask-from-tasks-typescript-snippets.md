---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TodoTask();
requestBody.title = "A new task";
const linkedresource = new LinkedResource();
linkedresource.webUrl = "http://microsoft.com";
linkedresource.applicationName = "Microsoft";
linkedresource.displayName = "Microsoft";
requestBody.linkedResources = [
			linkedresource
		]
const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasks.post(requestBody);
}


```