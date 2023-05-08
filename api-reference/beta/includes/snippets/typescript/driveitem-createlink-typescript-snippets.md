---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CreateLinkPostRequestBody = {
	type : "view",
	scope : "anonymous",
	password : "String",
	recipients : [
		{
			"@odata.type" : "microsoft.graph.driveRecipient",
		},
	],
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").createLink.post(requestBody);
}


```