---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GetMailTipsPostRequestBody
{
	EmailAddresses = new List<>
	{
		"danas@contoso.onmicrosoft.com",
		"fannyd@contoso.onmicrosoft.com",
	},
	MailTipsOptions = MailTipsType.Automaticreplies, mailboxfullstatus,
};
var result = await graphClient.Me.GetMailTips.PostAsync(requestBody);


```