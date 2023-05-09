---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MeetingRegistrantBase = {
	"@odata.type" : "#microsoft.graph.meetingRegistrant",
	additionalData : {
		"firstName" : "Frederick",
		"lastName" : "Cormier",
		"email" : "frederick.cormier@contoso.com",
		customQuestionAnswers : [
			{
				questionId : "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
				value : "No",
			},
			{
				questionId : "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
				value : "Internet",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").onlineMeetingsById("onlineMeeting-id").registration.registrants.post(requestBody);
}


```