---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthoredNote
{
	Content = new ItemBody
	{
		Content = "String",
		ContentType = BodyType.Text,
	},
};
var result = await graphClient.Privacy.SubjectRightsRequests["subjectRightsRequest-id"].Notes.PostAsync(requestBody);


```