---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["documents"],
	}
};

const result = async () => {
	await graphServiceClient.print.printersById("printer-id").jobsById("printJob-id").get(configuration);
}


```