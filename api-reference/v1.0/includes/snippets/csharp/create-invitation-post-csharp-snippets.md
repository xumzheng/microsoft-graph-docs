---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Invitation
{
	InvitedUserEmailAddress = "admin@fabrikam.com",
	InviteRedirectUrl = "https://myapp.contoso.com",
};
var result = await graphClient.Invitations.PostAsync(requestBody);


```