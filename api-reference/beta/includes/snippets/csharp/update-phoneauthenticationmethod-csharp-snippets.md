---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PhoneAuthenticationMethod
{
	PhoneNumber = "+1 2065555554",
	PhoneType = AuthenticationPhoneType.Mobile,
};
await graphClient.Me.Authentication.PhoneMethods["phoneAuthenticationMethod-id"].PatchAsync(requestBody);


```