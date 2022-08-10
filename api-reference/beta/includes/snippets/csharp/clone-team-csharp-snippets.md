---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ClonePostRequestBody
{
	DisplayName = "Library Assist",
	Description = "Self help community for library",
	MailNickname = "libassist",
	PartsToClone = ClonableTeamParts.Apps,tabs,settings,channels,members,
	Visibility = TeamVisibilityType.Public,
};
await graphClient.Teams["team-id"].Clone.PostAsync(requestBody);


```