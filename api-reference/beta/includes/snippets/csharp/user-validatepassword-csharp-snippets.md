---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Users.MicrosoftGraphValidatePassword.ValidatePasswordPostRequestBody
{
	Password = "1234567890",
};
var result = await graphClient.Users.MicrosoftGraphValidatePassword.PostAsync(requestBody);


```