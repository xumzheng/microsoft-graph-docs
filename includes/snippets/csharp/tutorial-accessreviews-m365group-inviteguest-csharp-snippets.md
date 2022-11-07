---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Invitation
{
	InvitedUserDisplayName = "John Doe (Tailspin Toys)",
	InvitedUserEmailAddress = "john@tailspintoys.com",
	SendInvitationMessage = false,
	InviteRedirectUrl = "https://myapps.microsoft.com",
};
var result = await graphClient.Invitations.PostAsync(requestBody);


```