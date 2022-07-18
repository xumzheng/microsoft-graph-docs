---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ItemPhone
{
	DisplayName = "Car Phone",
	Number = "+7 499 342 22 13",
};
var result = await graphClient.Me.Profile.Phones.PostAsync(requestBody);


```