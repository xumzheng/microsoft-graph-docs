---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ValidatePasswordPostRequestBody
{
	Password = "1234567890",
};
var result = await graphClient.Users.ValidatePassword.PostAsync(requestBody);


```