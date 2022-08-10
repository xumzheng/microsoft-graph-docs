---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingCustomQuestion
{
	OdataType = "#microsoft.graph.bookingCustomQuestion",
	DisplayName = "What is your age?",
	AnswerInputType = AnswerInputType.Text,
	AnswerOptions = new List<>
	{
	},
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].CustomQuestions.PostAsync(requestBody);


```