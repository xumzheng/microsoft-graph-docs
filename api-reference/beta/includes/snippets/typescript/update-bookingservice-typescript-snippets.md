---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingService = {
	"@odata.type" : "#microsoft.graph.bookingService",
	defaultDuration : "PT30M",
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").servicesById("bookingService-id").patch(requestBody);
}


```