---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChangePasswordPostRequestBody
{
	CurrentPassword = "xWwvJ]6NMw+bWH-d",
	NewPassword = "0eM85N54wFxWwvJ]",
};
await graphClient.Me.ChangePassword.PostAsync(requestBody);


```