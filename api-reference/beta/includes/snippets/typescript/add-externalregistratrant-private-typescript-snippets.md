---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MeetingRegistrantBase = {
	"@odata.type" : "#microsoft.graph.externalMeetingRegistrant",
	id : "30494ab7-7338-4592-bfec-a4333be2a0a6",
	additionalData : {
		"tenantId" : "909c6581-5130-43e9-88f3-fcb3582cde37",
		"userId" : "cc515404-b55c-466e-b896-992c918ecc01",
	},
};

const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.registrants.post(requestBody);
}


```