---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EmailAuthenticationMethod
{
	EmailAddress = "kim@contoso.com",
};
var result = await graphClient.Users["user-id"].Authentication.EmailMethods.PostAsync(requestBody);


```