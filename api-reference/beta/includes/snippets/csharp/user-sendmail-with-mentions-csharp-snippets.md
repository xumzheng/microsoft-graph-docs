---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SendMailPostRequestBody
{
	Message = new Message
	{
		Subject = "Project kickoff",
		ToRecipients = new List<Recipient>
		{
			new Recipient
			{
				EmailAddress = new EmailAddress
				{
					Name = "Samantha Booth",
					Address = "samanthab@contoso.onmicrosoft.com",
				},
			},
		},
		Mentions = new List<Mention>
		{
			new Mention
			{
				Mentioned = new EmailAddress
				{
					Name = "Dana Swope",
					Address = "danas@contoso.onmicrosoft.com",
				},
			},
		},
	},
};
await graphClient.Me.SendMail.PostAsync(requestBody);


```