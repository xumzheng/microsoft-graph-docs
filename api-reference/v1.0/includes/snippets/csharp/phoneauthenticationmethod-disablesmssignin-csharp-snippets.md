---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Me.Authentication.PhoneMethods["phoneAuthenticationMethod-id"].DisableSmsSignIn.PostAsync();


```