---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ForwardPostRequestBody
{
	ToRecipients = new List<Recipient>
	{
		new Recipient
		{
			EmailAddress = new EmailAddress
			{
				Address = "danas@contoso.onmicrosoft.com",
				Name = "Dana Swope",
			},
		},
	},
	Comment = "Dana, hope you can make this meeting.",
};
await graphClient.Me.Events["event-id"].Forward.PostAsync(requestBody);


```