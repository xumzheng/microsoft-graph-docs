---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["c300x400_crop"],
	}
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").thumbnails.get(configuration);
}


```