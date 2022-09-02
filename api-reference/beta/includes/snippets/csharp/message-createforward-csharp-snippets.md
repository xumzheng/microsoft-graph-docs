---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreateForwardPostRequestBody
{
	Message = new Message
	{
		IsDeliveryReceiptRequested = true,
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
	},
	Comment = "Dana, just want to make sure you get this; you'll need this if the project gets approved.",
};
var result = await graphClient.Me.Messages["message-id"].CreateForward.PostAsync(requestBody);


```