---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CustomQuestion
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.type" , "#microsoft.graph.bookingCustomQuestion"
		},
		{
			"displayName" , "What is your age?"
		},
		{
			"answerInputType" , "text"
		},
		{
			"answerOptions" , new List<>
			{
			}
		},
	},
};
await graphClient.BookingBusinesses["bookingBusiness-id"].CustomQuestions["bookingCustomQuestion-id"].PostAsync(requestBody);


```