---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ValidatePropertiesPostRequestBody
{
	EntityType = "Group",
	DisplayName = "Myprefix_test_mysuffix",
	MailNickname = "Myprefix_test_mysuffix",
	OnBehalfOfUserId = "onBehalfOfUserId-value",
};
await graphClient.DirectoryObjects.ValidateProperties.PostAsync(requestBody);


```