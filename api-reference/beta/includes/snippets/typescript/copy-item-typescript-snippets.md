---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CopyPostRequestBody = {
	parentReference : {
		driveId : "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
		id : "DCD0D3AD-8989-4F23-A5A2-2C086050513F",
	},
	name : "contoso plan (copy).txt",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").copy.post(requestBody);
}


```