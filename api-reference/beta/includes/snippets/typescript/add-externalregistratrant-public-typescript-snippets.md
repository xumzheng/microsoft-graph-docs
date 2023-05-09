---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MeetingRegistrantBase = {
	"@odata.type" : "#microsoft.graph.externalMeetingRegistrant",
	id : "9d96988d-a66a-46ce-aad7-0b245615b297",
};

const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.registrants.post(requestBody);
}


```