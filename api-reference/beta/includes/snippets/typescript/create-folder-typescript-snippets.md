---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DriveItem = {
	name : "New Folder",
	folder : {
	},
	additionalData : {
		"@microsoft.graph.conflictBehavior" : "rename",
	},
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").children.post(requestBody);
}


```