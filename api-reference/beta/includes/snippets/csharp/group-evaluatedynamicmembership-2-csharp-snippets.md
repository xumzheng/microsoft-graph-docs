---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EvaluateDynamicMembershipPostRequestBody
{
	MemberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33",
	MembershipRule = "(user.displayName -startsWith \"EndTestUser\")",
};
var result = await graphClient.Groups.EvaluateDynamicMembership.PostAsync(requestBody);


```