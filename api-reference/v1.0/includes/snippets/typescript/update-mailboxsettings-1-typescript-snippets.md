---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MailboxSettings = {
	automaticRepliesSetting : {
		status : AutomaticRepliesStatus.Scheduled,
		scheduledStartDateTime : {
			dateTime : "2016-03-20T18:00:00.0000000",
			timeZone : "UTC",
		},
		scheduledEndDateTime : {
			dateTime : "2016-03-28T18:00:00.0000000",
			timeZone : "UTC",
		},
	},
	additionalData : {
		"@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
	},
};

const result = async () => {
	await graphServiceClient.me.mailboxSettings.patch(requestBody);
}


```