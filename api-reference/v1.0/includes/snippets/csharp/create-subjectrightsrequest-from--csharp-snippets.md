---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SubjectRightsRequest
{
	Type = "microsoft.graph.subjectRightsRequestType",
	DataSubjectType = "microsoft.graph.dataSubjectType",
	Regulations = new List<String>
	{
		"String",
	}
	DisplayName = "String",
	Description = "String",
	InternalDueDateTime = DateTimeOffset.Parse("String (timestamp)"),
	DataSubject = new DataSubject
	{
		FirstName = "String",
		LastName = "String",
		Email = "String",
		Residency = "String",
		AdditionalData = new()
		{
			{"phoneNumber", "String"},
			{"SSN", "String"},
		}
	},
};
var result = await graphClient.Privacy.SubjectRightsRequests.PostAsync(requestBody);


```