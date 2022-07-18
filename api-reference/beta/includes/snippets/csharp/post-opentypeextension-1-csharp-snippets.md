---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Message
{
	Subject = "Annual review",
	Body = new ItemBody
	{
		ContentType = "HTML",
		Content = "You should be proud!",
	},
	ToRecipients = new List<Recipient>
	{
		new Recipient
		{
			EmailAddress = new EmailAddress
			{
				Address = "rufus@contoso.com",
			},
		},
	}
	Extensions = new List<Extension>
	{
		new Extension
		{
			@odata.type = "microsoft.graph.openTypeExtension",
			AdditionalData = new()
			{
				{"extensionName", "Com.Contoso.Referral"},
				{"companyName", "Wingtip Toys"},
				{"expirationDate", "2015-12-30T11:00:00.000Z"},
				{"dealValue", },
			}
		},
	}
};
var result = await graphClient.Me.Messages.PostAsync(requestBody);


```