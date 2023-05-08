---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InvitePostRequestBody = {
	recipients : [
		{
			email : "robin@contoso.org",
		},
	],
	message : "Here's the file that we're collaborating on.",
	requireSignIn : true,
	sendInvitation : true,
	roles : [
		"write",
	],
	password : "password123",
	expirationDateTime : "2018-07-15T14:00:00.000Z",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").invite.post(requestBody);
}


```